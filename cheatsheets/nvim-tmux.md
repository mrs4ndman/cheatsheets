# Them keybinds

#### Got most of the binds from [him](https://youtube.com/playlist?list=PLm323Lc7iSW_wuxqmKx_xxNtJC_hJbQ7R) 
#### and his [config files](https://github.com/ThePrimeagen/init.lua)

## VIM / NVIM base modal motions & keybinds

- ### COMMAND MODE:

    - :sav <filename> = Saves to filename & switches the buffer to <filename> 



- ### NORMAL:


    - h, j, k & l = move left, down, up and right character by character (can be used with motions)

    - d = "dd" deletes a line, but it can be combined with "t", "f", and "a" / "i"

    - D = Deletes from where the cursor is to the end of the line

    - c = "cc" changes an entire line (drops you in Insert mode), works like "d"

    - C = Changes from where the cursor is to the end of the line

	- x = The better way to delete characters

    - v = Puts you in visual mode, usually combined with motions

    - V = Puts you in visual mode, but selects by lines instead of words
	
    - r = Replaces the letter the cursor is on with the letter you press after

    - R = Puts you into replace mode, which allows you to overwrite (try it out)


    - \<\< = Indent an entire line backwards

    - \>\> = Indent an entire line forwards

    - \< = Can be combined with a selection / motion to indent backwards x number of lines

    - \> = Can be combined with a selection / motion to indent x number of lines

    - = = "==" indents the current line correctly

    - =ap = Indents the whole paragraph & surrounding whitespace


	- p = Pastes either the last thing yanked or deleted in the line above the cursor

    - P = Pastes either the last thing yanked or deleted in the line above the cursor

	- d$ = deletes from the cursor to the end of the line - 
	
	- 0 = deletes from the beginning of the line to the cursor


    - \<number>gg / \<number>G = Go to line \<number>
	
    - b & w = Go to the beginning & ending of a word / different text format (counts space as a word)

    - W = Jump to the next space-separated text

    - e = Go to the ending of a word 

    - gg = Go to the first line

    - G = Go to the last line

	- $ = Go to the end of the line
	
	- _ = Go to the start of the line
	
	- 0 = Go to the beginning character of the line

    - ^ = Go to the beginning word of the line


    - \* = Searches for other instances of the word

    - ; = When using t + <character>, go to the next instance of the specified character


    - zz to center the page based on the cursor's position


    - Ctrl + a = Iterate the number under the cursor

    - Ctrl + d = Goes half a page down / forward | Baja media página

    - Ctrl + u = Goes half a page up | Sube media página

    - Ctrl + f = Goes a full page down / forward | Baja una página entera

    - Ctrl + b = Goes a full page up / backward | Baja una página entera

    - Ctrl + g = Gets info about the file (name, size, route to it)



- #### MOTION COMBINATIONS

	- f\<char\> = Goes forward to the specified character in the line
		- Can be combined with x to eliminate certain characters
			 
	- t\<char\> = Jumps to right before the specified character in the line (e.g. > )
		- Used with t\<char\> or f\<char\>
			- , = Go to the previous instance (but right before it)
			- ; = Go to the next instance (but right before it)
			
	- F\<char\> = Goes backwards to the specified character in the line (e.g. <) 
		
	- T\<char\> = Jumps to right after the previous specified character in the line (e.g. = ) 
		- T\<char\> is a mirror of t\<char\>, same with f \& F
		- Used with T\<char\> or F\<char\>

- ##### Both t / T \& f / F can be used with d, c, y, v (visual mode) \& p

	- df\<char\> deletes From the cursor to the next specified character in the line 
	- dF\<char\> deletes From the cursor to the previous specified character in the line
	- dt\<char\> deletes from the cursor To right before the next specified character in the line
	- dT\<char\> deletes from the cursor To right after the previous specified character in the line 
	
	- vf\<char\> selects From the cursor to the next specified character in the line 
	- vF\<char\> selects From the cursor to the previous specified character in the line
	- vt\<char\> selects from the cursor To right before the next specified character in the line
	- vT\<char\> selects from the cursor To right after the previous specified character in the line 
	
	
	- yf\<char\> yanks From the cursor to the next specified character in the line 
	- yF\<char\> yanks From the cursor to the previous specified character in the line
	- yt\<char\> yanks from the cursor To right before the next specified character in the line
	- yT\<char\> yanks from the cursor To right after the previous specified character in the line 
	
	
	- cf\<char\> changes From the cursor to the next specified character in the line 
	- cF\<char\> changes From the cursor to the previous specified character in the line
	- ct\<char\> changes from the cursor To right before the next specified character in the line
	- cT\<char\> changes from the cursor To right after the previous specified character in the line 
	
	
	- pf\<char\> pastes From the cursor to the next specified character in the line 
	- pF\<char\> pastes From the cursor to the previous specified character in the line
	- pt\<char\> pastes from the cursor To right before the next specified character in the line
	- pT\<char\> pastes from the cursor To right after the previous specified character in the line


### INSERT:

- i = Enter insert mode right on the cursor
	- I = Enter insert mode, but position the cursor at the beginning of the line
- a = Enter insert mode, but right after the cursor
	- A = Enter insert mode, but right over the end of the line
- o = Enter insert mode, but in a new line below the one we're in
	- O = Enter insert mode, but in a new line above the one we're in
 

### VISUAL:


- y = "yy" yanks an entire line, but can be combined with a motion ( e.g "yiw" )

- % = Used like, for example, Vf(%, it selects from the { to its matching }
    - It allows you to jump between sets of characters ( {}, (), ' ', etc. )

- VD = Visually delete a whole line, technically faster than double tapping "d"
- VY = Faster way to do the same as 'yy'

- vi<delimiter> = Selects everything in between the delimiters ( {}, [], (), etc)
- va<delimiter> = Selects everything (like vi) in and around (including the delimiters)
- ya<delimiter> = Yanks with the same selection as va would do
- viw = Selects in visual mode the whole word, doesn't care about positioning
- viW = Same as viw but selects all text until there are whitespaces
- o = Alternates your cursor between the top / bottom of the current visual selection 
- vap & dap = They select / delete paragraphs AND the contiguous whitespace
- vip & dip = They select / delete only the insides of the paragraphs



## NVIM: Custom keybinds with space as leader & modal keybinds for easy motions

##### All related configs on [here](https://github.com/mrs4ndman/setup)

- #### (assuming Space is leader in neovim)
	
	- Leader + Leader = Source current file
	- Leader + b = Base binding for--
	    - Leader + b + n = Next buffer
	    - Leader + b + p = Previous buffer
	    - Leader + b + c = Buffer close / delete from list
	
    - Leader + c + t = Treesitter context toggle
    - Leader + c + x = Make the current file executable (chmod +x)
	- Leader + e = Ex (Nvim Integrated Explorer)
    - Leader + f + m + l = Cellular automaton effect keybind
    - Leader + m + d = Start up Glow markdown window

 
## Modal custom keybinds (not global)

- ### NORMAL:
	
	- J = append line below to current one
	- Q = Manually unbound in config (do not need it)
    - Leader + p / d: In visual / normal mode, paste and delete without picking the text into paste buffer
    - Ctrl + s = Substitutor
	
- ### INSERT:
	
	- Ctrl + c = Escape (i know, right?)

- ### VISUAL:
	
	- J \& K: Move selection completely up or down inside the buffer


- ### cokeline plugin [ .config/nvim/after/plugin/cokeline.lua ]
	
	- leader + c + n = focus on next buffer in the cokeline
	 
	- leader + c + p = focus on previous buffer in the cokeline
	 
	- leader + c + s + n = switch current buffer with the next buffer in the cokeline
	 
	- leader + c + s + p = switch current buffer with the previous buffer in the cokeline
	 
	- leader + c + c = pick (based on a letter index) which of the session buffers to close
	 
	- leader + c + \<number> = focus / change to the buffer with the buffer numbered \<number>
	 
	- Leader +  s + \<Number> = Switch the current buffer with the buffer numbered \<Number>


- ### Fugitive plugin [ .config/nvim/after/plugin/fugitive.lua ]
	
	- Leader + g + s = Fugitive git status
	- Leader + g + d = Fugitive git diff


- ### Harpoon plugin [ .config/nvim/after/plugin/harpoon.lua ]
	
    - Leader + h = harpoon main screen / plugin
    - Leader + a = harpoon mark keybinding

	- Leader + 1 = harpoon file 1
	- Leader + 2 = harpoon file 2
	- Leader + 3 = harpoon file 3
	- Leader + 4 = harpoon file 4
	- Leader + 5 = harpoon file 5
	- Leader + 6 = harpoon file 6
	- Leader + 7 = harpoon file 7
	- Leader + 8 = harpoon file 8
	- Leader + 9 = harpoon file 9
	- Leader + 0 = harpoon file 10
	
	- Leader + t + 1 = harpoon terminal 1
	- Leader + t + 2 = harpoon terminal 2
	- Leader + t + 3 = harpoon terminal 3
	- Leader + t + 4 = Harpoon terminal 4


- ### LSP keybinds
	
    - gd = Go to definition
    - K = Hover
    - [d / ]d = Go to next and previous diagnostic hunks
    - Ctrl + o = Bring up signature help
	- Ctrl + p = Previous LSP suggestion / item
	- Ctrl + n = Next LSP suggestion / item
	- Ctrl + y = Confirm selected suggestion / item
	- Ctrl + Space = Complete suggestion ??
    - Leader + vca = Choose and execute available code actions
    - Leader + vd = Open diagnostics in a floating window
    - Leader + vrn = Rename references to the symbol under the cursor 
    - Leader + vrr = View references
    - Leader + vws = View LSP workspace symbol


- ### Packer plugin manager
	  
	- Leader + p + s = Packer Sync

 
- ### Ranger / rnvimr plugin
	
	- Leader + r = Ranger with rnvimr plugin inside Neovim


- ### Surround plugin

    - c + s + current surrounding + new surrounding = Change current for new surrounding signs / marks
    - c + s + t = go back to previuos pair
    - d + s + current surrounding = Delete current surrounding delimiters / signs / marks
    - y + s + iw motion + surrounding = Add another surrounding inside the current one
    - y + s + s + b or ) = Wrap the entire line in parentheses
    - V + S + 'XML tag / surrounding' = this can surround the entire current line in the surroundig / XML tag

    - Only the opening brackets used with surround pad the surrounded text with a space
    - To surround without padding, use the closing brackets



- ### Overlength plugin

    - Leader + ol = Toggle overlength highlighting on / off


- ### Telescope plugin & extensions
	
    - Leader + t + f = Telescope plugin main screen
	- Leader + t + s = Live grep the file, telescope plugin
    - Leader + t + g = Telescope Git module
	- Leader + t + o = History of recently opened files, works with hidden folder files
    - Leader + v + h = View help tags
    - Inside of fuzzy finding window (works both in normal and insert modes) :
        - Ctrl + n = Next selection
        - Ctrl + p = Previous selection
        - Ctrl + c = Close window and return to working buffer
        - Ctrl + q = Send to quick-fix list
        - Ctrl + i = Select more in horizontal (??)
        - Ctrl + x = Select more in vertical (??)



- ### Trouble plugin
	
	- Leader + x + q = Trouble toggle quick-fix
	- Leader + x + w = Trouble workspace diagnostics 
	- Leader + x + x = Trouble full toggle
	- Leader + x + d = Trouble document diagnostics
	- Leader + x + l = Trouble location list

 
- ### Undotree plugin
	
	- Leader + u = Toggle Undo tree (pops window on the side)

- ### Vinegar plugin

    - Inside of Ex: What is inside quotes is the keybind
        - "-" = Go up a directory
        - I = Makes the Ex default top banner show
        - "." = Pre-populate a file at the end of a ":" command line
        - y. = Yank an absolute path for the file under the cursor
        - ~ = Go to $HOME
         - Ctrl + ^ = Go to previous buffer
    
- ### Zenmode plugin
	
	- Leader + zz = Zen mode
	- Leader + zZ = Zen mode without numbers and wrap


- ### Unbound
	
	- Leader + I = Nothing
	- Leader + D = Nothing
	- Leader + F = Nothing
	- Leader + J = Nothing
	- Leader + K = Nothing
	- Leader + L = Nothing
	- Leader + Ñ (or whatever is here in english) = Nothing
	- Leader + X = Nothing
	- Leader + N = Nothing 



- ### TMUX: Default keybinds
	
	- (assuming Ctrl + s as prefix / leader for Tmux)
	
	- #### Leader + ? = List all key bindings
	 
	- ### Most used:
	
	- ##### Layouts:
		- Leader + ( Alt + 1 ) = Even-horizontal layout
		- Leader + ( Alt + 2 ) = Even-vertical layout
		- Leader + ( Alt + 3 ) = Main horizontal layout
		- Leader + ( Alt + 4 ) = Main vertical layout
		- Leader + ( Alt + 5 ) = Tiled layout
	
	- Leader + ( Ctrl + Up / Down / Left / Right ) = Resize the current pane in 1-cell steps
	- Leader + ( Alt + Up / Down / Left / Right ) = Resize the current pane in 5-cell steps
	
	
	- ##### Panes:
		- Leader + [Ctrl + o] = Rotates the panes in the current window forwards 
		- Leader + q = Identify panes with numbers & show their indexes
		- Leader + % = Horizontally splits the current pane into left and right panes
		- Leader + " = Vertically splits the current pane into top and bottom panes
		- Leader + x = Kills the current pane
		- Leader + o = Select the next pane in the current window
		- Leader + ; = Move to the previously active pane
		- Leader + { / } = Swaps the current pane with the previous / next one
		- Leader + m / M = Mark current pane / Clear the marked pane


	- ##### Windows:
		- Leader + c = Create a new window
		- Leader + p = Previous window
		- Leader + n = Next window
		- Leader + [ 0 - 9 ] = Select windows 0 to 9
		- Leader + w = Opens window / pane selector dropdown menu
		- Leader + ! = Breaks into another window the current pane
		- Leader + & = Kill the current window
		- Leader + i = Current window info
		- Leader + f = Text search in open windows


	- ##### Config & features
		- Leader + [Ctrl + s] = Sends prefix to the application
		- Leader + t = CLI-rendered clock
		- Leader + z = Toggles zoom / focus mode
		- Leader + r = Reload tmux.conf
		- Leader + : = Enter the tmux command prompt
		- Leader + [Ctrl + z] = Suspends the tmux client


	- ##### Sessions & clients
		- Leader + $ = Rename the current session
		- Leader + d / D = Detach the current client / Choose a client to detach
		- Leader + s = Select a new session for the attached client interactively
		- Leader + ( / ) = Switch the attached client to the previous or next session


	- ##### Paste buffers
		- Leader + # = List all paste buffers
		- Leader + "=" = Choose which buffer to paste interactively from a list 
		- Leader + - = Delete the most recent copied buffer of text


- ### TMUX: Custom keybinds

    - Ctrl + a = Prefix for tmux commands
    - Prefix + r = Re-sources the .tmux.conf config file
    - Prefix + h = Splits the window into 2 "horizontal" halves (vertical division)
    - Prefix + v = Splits the window into 2 "vertical" halves (horizontal division)
    - Prefix + i = Run tmux.cht.sh script (copied from ThePrimeagen's tmux setup)
    - Prefix + f = Run tmux-sessionizer script (copied from ThePrimeagen's tmux setup)
    - Prefix + D = Run tmux-sessionizer for quick access to dotfiles
    - Prefix + G = Run tmux-sessionizer for quick access to Github folder
    - Prefix + S = Run tmux-sessionizer for quick access to setup git repo
    - Prefix + ^ = Go to last window
    - Prefix + Prefix = Sends the prefix key combination (Ctrl + A) to the program below tmux