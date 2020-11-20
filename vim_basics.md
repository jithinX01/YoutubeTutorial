## Vim Basics and Shortcuts for beginners 

###### edit mode.

```shell
i #press key i, Press Escape to go back to view mode.
```

###### exit or quit vim

```shell
Escape , :q # Esc Key then :q
```

###### save content.

```shell
Escape , :w # save file
:wq #save and exit from vim
```

###### undo

```shell
Escape, :u
```

###### redo

```
Escape, Ctrl + r
```

###### move cursor by words

```shell
Ctrl+Left or Ctrl+Right
```

###### copy paste a line.

```shell
Escape , yy # Esc Key, move cursor to line to copy, press yy, This will copy line.
p #move cursor to a line before pasting, then press p.
```

###### copy n number of lines.

```shell
Escape, 10, yy # Esc Key, move cursor to lines to copy, press 10, then yy for 10 lines to copy
```

###### delete or cut a line

```shell
Escape , dd # Esc Key, move cursor to line to delete/cut, press dd, This will cut/delete line.
p # #move cursor to a line before pasting, then press p to paste.
Escape , 10, dd #cut 10 lines from cursor.
```

###### go to nth line.

```shell
Escape, :10 #go to 10th line
```

###### search/find

```shell
Escape, /searchpattern, Enter #search from cursor to botton
n # move cursor to next search
N # move cursor to previous search
Escape, ?searchpattern, Enter #backward search.
```

###### search and replace

```shell
Escape, :s/foo/bar/gc #Find each occurrence of 'foo' (in the current line only), and replace it with 'bar'.
:%s/foo/bar/gc # Find each occurrence of 'foo' (in all lines), and replace it with 'bar'.
:.,$s/foo/bar/gc 	#Change each 'foo' to 'bar' for all lines from the current line (.) to the last line ($) inclusive, optiong gc ask for confirmation
```

###### word suggestion

```shell
#in insert mode.
Ctrl + p #start typing a letter and press Ctrl+p vim will suggest, move up and down to select suggetion.
```

###### scroll down several lines

```shell
Ctrl + d
```

###### scroll up several lines

```shell
Ctrl + u
```

###### go to top of file.

```
Escape, gg
```

###### go to bottom of file.

```
Escape, G
```

#### VIDEO

[Vim Basics](https://www.youtube.com/watch?v=X93D0uSQnFo)

Note: Press Escape only if vim is in insert mode.