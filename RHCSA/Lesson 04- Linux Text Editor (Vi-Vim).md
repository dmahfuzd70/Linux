 Linux Text Editor:
-------------------
	 Windows Text Editor: notepad, notepadd++
	 Linux Text Editor: vi/vim, nano, gedit (GUI), emacs, pico

	  Most propular/Advanced Text Editor: Vi/Vim
		=> vi - old, b&w, default
		=> vim - advanced, colorfull (Package must be installed)

	 [student@hostX ~]$ cd
	 [student@hostX ~]$ mkdir linux/lesson04 -p
	 [student@hostX ~]$ cd linux/lesson04
	 [student@hostX lesson04]$ ls
	 [student@hostX lesson04]$ touch test          ; create new file
	 [student@hostX lesson04]$ cp /etc/passwd  .   ; copy passwd file to cureent dir
	 [student@hostX lesson04]$ ls
	  	passwd  test

	 [student@hostX lesson04]$ vim file1    ; edit newfile 
	 	welcome to vim editor

	 :x 

	 [student@hostX lesson04]$ cat file1

	 [student@hostX lesson04]$ nano file2
	 	welcome to nano editor

	 => Ctrl+X then 'Y'

	 [student@hostX lesson04]$ cat file2

	 [student@hostX lesson04]$ gedit file3

	 welcome to graphical geditor 

	 [student@hostX lesson04]$ cat file3

 Working with vi/vim Mode:
 ------------------------
	=> Insert Mode : press "i" or "insert" button
        => Exit Mode : press "esc" button form keyboard
        => Command Mode: file navigation, cut, paste, undo, redo
	=> Visual Mode: press "ctrl + v" form keyboard
 
	 [student@hostX lesson04]$  vim file4

	=> Press "i" for insert mode
	=> write something as your requirments ; (Hello world !!)
	=> press "esc" button exit from "insert" mode
	=> :x		; save and quit

	[student@hostX lesson04]$ ls
	[student@hostX lesson04]$ cat file4
  	Hello world !!

	[student@hostX lesson04]$ vim file4

	=> Press "i" for insert mode
	=> write "welcome to linux training"
	=> press "esc" quit from insert mode
  	=> :w	; only save not quit

	=> Press "i" for insert mode
	=> write "goodbye" 

	=> :q! 	 ; quit without save

	[student@hostX lesson04]$ cat file4

	[student@hostX lesson04]$  vim passwd
	:set nu

Cursor Movement:
----------------
   	h j k l 	- Left, down, up, right
   	^ 		- Go to the beginning of the line
   	$ 		- Go to the end of the line
   	gg 		- Go to the frst line
   	G 		- Go to the last line
   	:n 		- Go to line n

Replacing Text:
---------------
   	r 		- Replace character
 
Copy/Paste:
-----------
   	yw        -  word copy
   	yy 	     -  Yank line

   	nyy 	     -  n lines copy   
   	p         -  Paste after cursor
   	P 	     -  Paste before cursor

Inserting Text:
---------------
	i 		- Insert at cursor
	I 		- Insert at the beginning of the line
	a 		- Append after cursor
	A 		- Append at the end of the line
	o 		- Open a new line below the current line
	O 		- Open a new line above the current line

Deleting Text:
--------------
	x  		- delete (cut) character
	dd 		- delete (cut) line
	ndd           - delete (cut) n lines 
	dw 		- delete (cut) word
	D             - delete (cut) to the end of the line

Undo/Redo:
---------
	u 	- Undo
	Ctrl-r 	- Redo

Searching:
----------
	/{pattern}	- Forward search for {pattern}
	?{pattern} 	- Reverse search for {pattern}
	n 		- Repeat the last search
	N 		- Repeat the last search in the opposite direction

Find and Replace:
-----------------
	:%s/{old}/{new}/gc  - Search and Replace with confirmation  
	:%s/{old}/{new}/g  - Search and Replace without confirmation  

Save and Quit:
-------------
	:w 	    - Write (save)
	:wq or :x  - Write and quit
	:q 	    - Quit
	:q! 	    - Force quit, don’t save changes
	:wq! 	    - Force write and quit

 	#vimtutor

 ======================== Thank you ===================

























