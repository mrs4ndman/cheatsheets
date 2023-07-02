# Them keybinds

#### Got most of the binds from [him](https://youtube.com/playlist?list=PLm323Lc7iSW_wuxqmKx_xxNtJC_hJbQ7R) 
#### and his [config files](https://github.com/ThePrimeagen/init.lua)

## VIM / NVIM base modal motions & keybinds

#### Actions → keys that, when pressed twice, have an effect on text editing. Can be combined with motions to get a broader range of action
#### Motions → keys that, when pressed, can be stacked together with actions to modify text in greater ways
#### Mode → The status in which the editor and keys operate. Can be changed by keybinds, and have different purposes

### Modal keys
#### Visual mode

- <kbd>v</kbd> → Puts you in visual mode, usually combined with motions
- <kbd>V</kbd> → Puts you in visual mode, but selects by lines instead of words
<br>

#### Insert mode

- <kbd>i</kbd> = Enter insert mode to the left on the cursor
- <kbd>I</kbd> = Enter insert mode at the beginning of the line
<br>

- <kbd>a</kbd> = Enter insert mode, but to the right of the cursor
- <kbd>A</kbd> = Enter insert mode at the end of the line
<br>

- <kbd>o</kbd> = Enter insert mode, but in a new line below
- <kbd>O</kbd> = Enter insert mode, but in a new line above
<br>

#### Command mode

- <kbd>:</kbd> = Enter command mode
- <kbd>:sav <filename></kbd> = Enters command mode and saves to `filename` & switches the buffer to it
<br> 

### NORMAL:

#### Actions by themselves, motions when combined with specific keys
- <kbd>h</kbd>, <kbd>j</kbd>, <kbd>k</kbd> & <kbd>l</kbd> = move left, down, up and right character by character (can be used with motions)
<br>

- <kbd>$</kbd> = Go to the end of the line
- <kbd>\_</kbd> = Go to the start of the line
<br>

- <kbd>0</kbd> = Go to the beginning character of the line
- <kbd>^</kbd> = Go to the beginning word of the line
<br>

#### Available motions

- <kbd>=ap</kbd> = Indents the whole paragraph & surrounding whitespace
<br>
- <kbd>d$</kbd> = deletes from the cursor to the end of the line
<br>

#### Available actions
##### Basic text manipulation
- <kbd>d</kbd> = "dd" deletes a line, but it can be combined with "t", "f", and "a" / "i"

- <kbd>D</kbd> = Deletes from where the cursor is to the end of the line
<br>

- <kbd>c</kbd> = "cc" changes an entire line (drops you in Insert mode), works like "d"
- <kbd>C</kbd> = Changes from where the cursor is to the end of the line
<br>

- <kbd>x</kbd> = The better way to delete characters
<br>

- <kbd>r</kbd> = Replaces the letter the cursor is on with the letter you press after
<br>

- <kbd>p</kbd> = Pastes either the last thing yanked or deleted in the line above the cursor

- <kbd>P</kbd> = Pastes either the last thing yanked or deleted in the line above the cursor
<br>

- <kbd>d$</kbd> = deletes from the cursor to the end of the line

- <kbd>0</kbd> = deletes from the beginning of the line to the cursor
<br>


##### Indentation management
- <kbd><</kbd> = Can be combined with a selection / motion to indent backwards x number of lines
- <kbd>></kbd> = Can be combined with a selection / motion to indent x number of lines
<br>

- <kbd><<</kbd> = Indent an entire line backwards
- <kbd>>></kbd> = Indent an entire line forwards
<br>

- <kbd>=</kbd> = Motion target, "\=\=" indents the current line correctly
- <kbd>=ap</kbd> = Indents the whole paragraph & surrounding whitespace
<br>

##### Viewspace navigation
- <kbd>L</kbd> = Go to the bottom of the currently visible text    	

- <kbd>H</kbd> = Go to the top of the currently visible text   	

- <kbd>M</kbd> = Go to the middle of the currently visble text
<br>

##### Line navigation
- <kbd>gg</kbd> = Go to the first line

- <kbd>G</kbd> = Go to the last line

- <kbd>Xgg</kbd> / <kbd>XG</kbd> = Go to line X
<br>

##### Word manipulation
- <kbd>b</kbd> & <kbd>w</kbd> = Go to the beginning & ending of a word / different text format (counts space as a word)

- <kbd>W</kbd> = Jump to the next space-separated text

- <kbd>e</kbd> = Go to the ending of a word 
<br>

- <kbd>`*`</kbd> = Searches for other instances of the word

- <kbd>zz</kbd> to center the page based on the cursor's position
<br>

- <kbd>Ctrl + a</kbd> = Iterate the number under the cursor

- <kbd>Ctrl + d</kbd> = Goes half a page down / forward | Baja media página

- <kbd>Ctrl + u</kbd> = Goes half a page up | Sube media página

- <kbd>Ctrl + f</kbd> = Goes a full page down / forward | Baja una página entera

- <kbd>Ctrl + b</kbd> = Goes a full page up / backward | Baja una página entera

- <kbd>Ctrl + g</kbd> = Gets info about the file (name, size, route to it)



#### MOTION COMBINATIONS

- <kbd>f\<char\></kbd> = Goes forward to the specified character in the line
	- Can be combined with x to eliminate certain characters

- <kbd>t\<char\></kbd> = Jumps to right before the specified character in the line (e.g. > )
	- Used with t\<char\> or f\<char\>

- <kbd>F\<char\></kbd> = Goes backwards to the specified character in the line (e.g. <) 

- <kbd>T\<char\></kbd> = Jumps to right after the previous specified character in the line (e.g. = ) 
	- T\<char\> is a mirror of t\<char\>, same with f \& F
	- Used with T\<char\> or F\<char\>

- <kbd>,</kbd> = Go to the previous instance (but right before it)
	- <kbd>;</kbd> = Go to the next instance (but right before it)

##### Both t / T \& f / F can be used with d, c, y, v (visual mode) \& p

- <kbd>df\<char\></kbd> deletes From the cursor to the next specified character in the line 
- <kbd>dF\<char\></kbd> deletes From the cursor to the previous specified character in the line
- <kbd>dt\<char\></kbd> deletes from the cursor To right before the next specified character in the line
- <kbd>dT\<char\></kbd> deletes from the cursor To right after the previous specified character in the line 

- <kbd>vf\<char\></kbd> selects [F]rom the cursor to the next specified character in the line 
- <kbd>vF\<char\></kbd> selects From the cursor to the previous specified character in the line
- <kbd>vt\<char\></kbd> selects from the cursor To right before the next specified character in the line
- <kbd>vT\<char\></kbd> selects from the cursor To right after the previous specified character in the line 


- <kbd>yf\<char\></kbd> yanks From the cursor to the next specified character in the line 
- <kbd>yF\<char\></kbd> yanks From the cursor to the previous specified character in the line
- <kbd>yt\<char\></kbd> yanks from the cursor To right before the next specified character in the line
- <kbd>yT\<char\></kbd> yanks from the cursor To right after the previous specified character in the line 


- <kbd>cf\<char\></kbd> changes From the cursor to the next specified character in the line 
- <kbd>cF\<char\></kbd> changes From the cursor to the previous specified character in the line
- <kbd>ct\<char\></kbd> changes from the cursor To right before the next specified character in the line
- <kbd>cT\<char\></kbd> changes from the cursor To right after the previous specified character in the line 


- <kbd>pf\<char\></kbd> pastes From the cursor to the next specified character in the line 
- <kbd>pF\<char\></kbd> pastes From the cursor to the previous specified character in the line
- <kbd>pt\<char\></kbd> pastes from the cursor To right before the next specified character in the line
- <kbd>pT\<char\></kbd> pastes from the cursor To right after the previous specified character in the line


### INSERT:

- <kbd>i</kbd> = Enter insert mode right on the cursor
- <kbd>I</kbd> = Enter insert mode, but position the cursor at the beginning of the line
    
- <kbd>a</kbd> = Enter insert mode, but right after the cursor
- <kbd>A</kbd> = Enter insert mode, but right over the end of the line
    
- <kbd>o</kbd> = Enter insert mode, but in a new line below the one we're in
- <kbd>O</kbd> = Enter insert mode, but in a new line above the one we're in
    
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

