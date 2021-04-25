# Magic
A shell script capable of altering aspects of the window manager, in the visual part, changing the colors of the gtk propio theme, of bars such as polybar and tint2, also changes colors of terminals such as termite, urxvt, xterm and others.

![](https://github.com/Paladin1991/Magic/blob/main/exemplo.gif)

### Dependencies

**Few dependencies are necessary for the operation of this script**  

* feh  
To set backgrounds. The script uses  
".fehbg" to identify the current background.  
[Feh](https://github.com/derf/feh)

* imagemagick  
So that it is possible to capture the background colors  
[ImageMagick](https://imagemagick.org/script/index.php)

* python-colr  
For the selected colors to be displayed on the terminal.  
[Colr](https://pypi.org/project/Colr/)  

##  How to use  

At the moment this script works only in my settings,  
because I did it for my own use, to make things easier for me.  
It works well on.  

* Xmonad + Polybar  
These are my xmonad configurations with polybar.  
[Dotfiles Xmonad](https://github.com/Paladin1991/dotfiles.xmonad)

* Fvwm + Tint2  
These are my settings for Fvwm with Tint2.  
[Dotfiles Fvwm](https://github.com/Paladin1991/dotfiles.fvwm)  

* Herbstluftwm + Tint2  
These are my settings for Herbstluftwm with Tint2.  
[Dotfiles Herbstluftwm](https://github.com/Paladin1991/dotifiles.herbstluftwm)

Although I use the bars in this way,  
and have specified above so,  
nothing prevents using polybar ao instead of tint2,  
the script is able to recognize the bar being used and modify only it.  

## Procedures.  

Usage is quite simple as shown in the GIF above.  
You must first install the window manager you want,  
as long as it is one of the 3 above.  
If you already have one installed and configured,  
make a backup of its settings, in case you want to use it in the future.

1. Choose one of the dotfiles above and clone.  
2. Run the small "install.sh" script contained within the script folder.  
3. Restart your window manager.  

## Using the script.  

First, in a terminal, you must navigate to where the script is located.  
Run the **sh magic** command,  
and follow the steps, always paying attention to what is written.

## Phases

1. Say whether you want the script to capture the colors of the current background.  
2. Tell the script how many colors it should capture.  
3. Choose if you would like to save the captured colors in a file located in your home,  
with the name "colors.txt"

#### All steps can be skipped by answering "n" (No), or by pressing (Enter) in step number one.

4. Choose the colors that will be used as the base "Background" of the theme.  
5. Choose the color that will be used as the highlight in the theme.  
6. Choose the color that will be used in the theme texts.  
7. In this step, the current colors of the theme will be displayed,  
as well as the colors you have chosen.  
Compare them and answer "y" (Yes) to apply the changes.  

Read carefully the possible warnings that the script can give,  
and in no way use similar colors, as this can cause problems.  

## Something went wrong.

There is a possibility that something goes wrong,  
due to a script failure or human speech. If this happens don't worry,  
run the program again and choose different colors,  
everything will be fine. If nothing is resolved,  
you can fix it manually in the configuration scripts.  

## Bugs

[] For no apparent reason, the program uses only one color in all instances,  
often decaying the background  
colors of the same color as the text.



