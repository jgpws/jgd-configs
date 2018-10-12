# jgd-configs
Various configuration files for Linux, pulled from my local desktop setup.

## How to Use:

### X11 Themes

This repository includes an .Xresources example. An .Xresources file is used for controlling how X11 applications, such as terminals, appear and function on the Linux desktop.

You may already have created an .Xresources file or may not have one. If you don't have an .Xresources file, you can right-click the .Xresources link and **Save Link as** to your Downloads folder, then move the file to your home folder (**home/_user_**) with a file manager/command line. Then follow steps 3 through 7 below to get the actual themes.

If you already have an existing .Xresources file, the method from this file will make X11 settings pluggable, whereas you can change X11 themes by commenting/uncommenting the include file for a theme. For convenience, I've placed the themes in an **x11-themes** directory.

1. Copy all of your existing configuration information in your .Xresources file (if it exists)
2. Create an **x11-themes** directory in your home directory (**home/_user_/x11-themes**)
3. Create a new file inside the x11-themes directory and name it something like **Default**; Paste into this file and Save
4. Right-click and save the links from this repository's **x11-themes** directory
5. Move the file from its download location (usually a Downloads folder) to your *local* x11-themes directory
6. In your local x11-themes directory, type `#include "x11-themes/name-of-theme"`
7. Comment out the theme you want to use, one at a time (Remove !)
8. If necessary, at the command line, type **xrdb ~/.Xresources** to save changes, then close and reopen an x11 program (xterm, for instance)

The themes included so far require **Bitstream Vera Sans Mono** and **DejaVu Sans Mono** fonts.

Once you have a folder for themes setup, you can include other color themes and place them in the folder, and add a new #include statement in your .Xresources file. An example follows below:

```
#include "x11-themes/jgd-classic"
!#include "another-directory/new-theme"
```

### Tint2 panel themes

To use tint2 themes, simply go to this repository's **tint2** directory, right-click the theme (with a .tint2rc extension), **Save Link As..** to your local computer. Then, move (Cut and Paste) the file to your local tint2 directory, located at **home/_user_/.config/tint2**.

With this being a new repository, I will add more themes/configuration files here in the future.
