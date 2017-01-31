# jgd-configs
Various configuration files for Linux, pulled from my local setup.

##How to Use:

###X11 Themes

This file includes an .Xresources example. .Xresources is used to control how X11 applications, such as terminals, appear and function on your Linux desktop.
You may already have created an .Xresources file or not have one. If you don't have an .Xresources file, you can right-click the .Xresources link and **Save Link as** to your Downloads folder, then move the file to your home folder (**home/_user_**) with your file manager. Then follow steps 3 through 6 below to get the actual themes.

If you already have an existing .Xresources file, the method in this file will make X11 themes pluggable, whereas you can change X11 themes by commenting/uncommenting the include file for a theme. For convenience, I've placed themes in an **X11-themes** directory.

1. Click .Xresources
2. Highlight lines that begin with #include, **Copy**, **Paste** into your local .Xresources file
3. Create **X11-themes** directory in your home directory (**home/_user_/x11-themes**)
4. Right-click and save links in this repository's **x11-themes** directory
5. Comment out the theme you want to use, one at a time
6. If necessary, at the command line, type **xrdb ~/.Xresources** to save changes, then close and reopen an x11 program (xterm, for instance)
