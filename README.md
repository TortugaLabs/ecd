# ecd

Enhanced cd (ecd) combines the functinionality of several builtin
shell commands for changing the current directory. It has all the
features of cd, pushd, and popd, while adding some additional
features. It can automatically execute certain scripts when entering
or leaving a directory, and it maintains a menu-driven history list to
assist in changing to prior directories.

Since it is implemented as a shell function, it resides in the shell's
memory and executes with no visible delay. And since functions do not
fork a subprocess, all executed commands are able to affect the
current shell.

Change the current directory to DIR, searching for hidden files named
`.enterrc' and `.exitrc'. Maintain a menu-driven history list to assist in
changing to prior directories.

The .enterrc/.exitrc idea is borrowed from Jerry Peek's Power Tools article
14.14. It expands on this idea by searching all subdirectories of the
destination directory having an uncommon base.

* * *



