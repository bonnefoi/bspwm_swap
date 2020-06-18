# bspwm_swap or "Swapping is not Swallowing"
This a solution to allow bspwm to **swap** the terminal window with the window of the program that you launch from it.

*This script use the hidden state of a window maintained by bspwm to hide the terminal window and swap its position with the window created by the last command.*

*It uses the *events* provided by **bspwm** to watch when the window of the last command is closed to unhide the terminal's window.*

You use the script by launching it with the command as arguments:
```
$ swap sxiv my_picture.jpg
```

You could also use the provided **zsh widget** to use a shortcut to substitute the return key by <ctrl-p> to change the behavior of the command:
```
$ sxiv my_picture.jpg <return>
```
launches the command without swapping: the window of the command is added to your current desktop.
```
$ sxiv my_picture.jpg <ctrl-p>
```
launches the command with swapping: the window of the command replace the terminal window until its ending.

You could also rename the script as "sins", 'Swapping Is Not Swallowing" if you want :)

*Another version of the script called ```other_version``` uses the pid of the launched command to unhide the terminal's window but don't use any events. This version exhibits a little bit of flickering as the window is closed before the command exits.*
