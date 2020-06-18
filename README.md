# bspwm_swap or "Swapping is not Swallowing"
This a solution to allow bspwm to **swap** the shell's window with the window of the program that you launch from it.

*This script use the hidden state of a window maintained by bspwm to hide the shell's window and swap its position with the window created by the last command.*

*It uses the *events* provided by **bspwm** to watch when the window of the last command is closed to unhide the shell's window.*

You use the script by launching it with the command as arguments:
```
$ swap sxiv my_picture.jpg
```

You could also use the provided zsh widget to use a shortcut to substitute the return key by <ctrl-p> to change the behavior :
```
$ sxiv my_picture.jpg <return>
```
launches the command without swapping.
```
$ sxiv my_picture.jpg <ctrl-p>
```
launches the command with swapping.

You could also rename the script as "sins", 'Swapping is not swallowing" if you want :)
