Custom Commands
===============

This is a repository for any custom commands, shortcuts, or lightweight scripts I come across or create. As of this first push, it has just one very helpful item:

bls
---

bls, or "better ls", is a command shortcut to print a much more readable list of files in the current directory than ls would normally do. Add this file to your /usr/bin, and provide it execute permissions. (or just symbolically link it.) Doing so will print a list of files in the current directory when you type 'bls':
* containing files with prefix "."
* in a single column list
* with prepended tab characters to help separate the list visually from the rest of the terminal
* with colorized filenames
* with "/" after directory names
* with "*" after executable names
* in case-insensitive sorted order
* with directories and executables appearing first

Note: bls uses the env variable "CLICOLOR_FORCE" to accomplish colorized output from ls in spite of the pipes. If you mind this side effect, you could add a line CLICOLOR_FORCE=0 in bls to reset the env variable after it's used. 

Other Note: I made bls using the OS X version of ls and sort, so it might not work on non-OSX.
