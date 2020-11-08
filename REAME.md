 

### XFCE4 launcher for WSL Bash with Vcxsrv

**OVERVIEW**

This is a template directory to launch XFCE with kali or ubuntu on WSL. The session will be launched quietly with the help of a windows script object

The shortcut is not portable to another directory and that is by design. I prefer all the related files in one place. If you wish, you may change the PATH to the scripts in the vbs and bat. Although, the way the windows script is run, you may run into relative/absolute path problems.

**IMPLEMENTATON NOTES**

- The pid of the server is checked so it’s not run twice.
- (gpg|ssh)-agent is killed before restarting the server on a second run
- LIBGL_ALWAYS_INDIRECT is defined for opengl via windows
- DISPLAY is set to “:0.0”

**RUNNING**

To run XFCE4, use “START XFCE4”