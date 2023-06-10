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
    
- Ctrl + P = Match string with next similar string
    
- Ctrl + N = Match string with previous similar string
 

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

