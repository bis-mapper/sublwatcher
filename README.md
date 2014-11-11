
# SUBLWATCHER - BIS file watching utility / IDE environment

<img src="https://raw.github.com/bis-mapper/sublwatcher/master/Docs/Images/sublwatcher.png" border="0">

## Initial Requirements 

In order to use this you must first install Sublime Text, Package Control, and Growl.

## Sublime Text
[Sublime Text](http://www.sublimetext.com/3)
* Download and install.  

## Package Control
[Package Control](https://sublime.wbond.net/installation)
* Follow install instructions on page.

## Growl for Windows
[Growl Download](http://www.growlforwindows.com/gfw/d.ashx?f=GrowlInstaller.exe)
* Follow setup instructions
* Once installed open up the growl GUI interface (System Icon tray in windows)
* You can set your default Displays and check to start program when computer is booted. 

## SUBLWATCHER - Load Application Package (File Watching Utility)

1. Download application package [Download](https://github.com/bis-mapper/sublwatcher/archive/master.zip)
2. Unzip file to folder.
3. Sign on as MAPCOORD.
4. Run PCME
5. Click -> Setup -> System Administration
6. Then -> Setup -> Load Application Package
7. Browse to the folder where you unzipped the application package.
8. Open the SETUP.RUN file -> Click Ok
9. The wizard will guide you through the rest of the steps.

## Install Sublime Plugins 

Open up Sublime Text and type in the following commands:

* Type `ctrl + shift + p`

* Then `pcar`

* Select *Package Control: Add Repository*

* copy and paste the URL *https://github.com/bis-mapper/bis-sublime* into the input field
at the bottom of the screen.

## Install package

* Type the following commands: `ctrl + shift + p`

* Then `pcip`

* Then select *bis-sublime* from the list

* Hit enter

## To Enable Color Scheme

Preferences -> Color Scheme -> bis-sublime -> BisColorScheme

# Getting Started (First Time Only)

Type `SUBL` on a report that you want to open.  (Try it with 2b0)

You will get prompted with a dialog box asking you to find the *sublime_text.exe*.
This should be stored in your program files where you installed Sublime.
Navigate to that folder and select the *sublime_text.exe*
Usually `c:\program\program files\sublime text 3\sublime_text.exe`

<img src="https://raw.github.com/bis-mapper/sublwatcher/master/Docs/Images/first_time.png" border="0">

## Windows folder location (File Watching Folder)

Some files are downloaded to your workstation when you run the `SUBL` command.  These files are stored in the sublwatcher folder 
`%USERPROFILE% usually c:\users\winne\sublwatcher\`

A browse utility will pop up asking you where you want to put the file that your opening.
<img src="https://raw.github.com/bis-mapper/sublwatcher/master/Docs/Images/browse.png" border="0">

Browse to your sublwatcher folder and select the folder for the site that your currently on.
<img src="https://raw.github.com/bis-mapper/sublwatcher/master/Docs/Images/select_folder.png" border="0">

The BIS report that you typed `SUBL` on will now be saved in this folder and you should be able to modify this file in Sublime and have the changes saved back to BIS.

## Watching Files
You can also type `SUBLWATCHER` on the control line to start the file watching utility.  This skips the process of opening up a specific report and starts the script that watches the files.  This is helpful if you already have the files you want open and just need to start saving the changes back to MAPPER.

## Additional Functionality and Commands

#### Open up the "BIS Control Line" in sublime

In Sublime Text type the following commands `Ctrl + Shift + o`

This will open up the "Bis Control Line"
<img src="https://raw.github.com/bis-mapper/sublwatcher/master/Docs/Images/control-line.png" border="0">

On this line you can type a report that you want to open just as you do in MAPPER (i.e. 2B0)  Hit enter on your keyboard to open up the report.

"Bis Control Line" features

* Open a Report
    - `ctrl + shift + o`
    - `2b0` to open up that report
* Dif
    - **Usage**
    - `ctrl + shift + o`
    - `dif` alone will do a dif between the file in Windows and the same file in MAPPER
    - `dif 2b56` you can also pass in another report after dif and it will compare it with that report
* SBS - Standardize BIS Script
    - **Usage**
    - `ctrl + shift + o`
    - `sbs` will run the SBS utility.
    - You can change your "standardize run" settings in 99d.
* Export - Export entire category, or just a specific drawer to a folder on your machine. 
    - **Usage**
    - `ctrl + shift + o`
    - `export 56 -f Sublwatcher` Exports the entire category into a folder of your choice, set by the -f option
    - `export f56 -f Sublwatcher` Exports only drawer F in category 56 to a folder of your choice.
    - `export b56 -f Sublwatcher` Exports only drawer B in category 56 to a folder of your choice.

####  BIS ERB - An easy way to wrap variables in the HTML output area.
`ctrl + shift + .` will wrap a variable like this `<%<VAR>(p)%>` saves you a few extra keystrokes

#### Help on a command or <html> tag

Highlight a BIS cmd like @srh or @tot and press `ctrl + shift + h` this should pop open the Unisys help document and bring you to that command.  Not all commands are referenced in here, so it may bring it up without the command selected.

This also works on html tags.  Highlight a `<div>` tag on your page and it will bring up the MDN (Mozilla Developer Network) documentation explaining this tag.


## Shortcuts

[Shortcut Reference](http://sublime-text-unofficial-documentation.readthedocs.org/en/latest/reference/keyboard_shortcuts_win.html)
[functionality demo](http://www.sublimetext.com/)

#### Line Operations

* Duplicate Line `ctrl + shift + d`
* Delete to end of line `ctrl + shift + delete`
* End of line `end`
* Beginning of line `home`
* Delete from cursor to beginning of line `ctrl + backspace`
* Move line up / down `ctrl + shift + up/down arrow keys`

#### Find operations
* Find in Files `ctrl + shift + f` ** Very handy **
* Find and replace `ctrl + h`
* Find anything `ctrl + p` (Brings up box where you can type in what your looking for)...

#### File Operations
* Save file `ctrl + s`
* Close file `ctrl + w`
* Open file `ctrl + o`

#### Add Folder to Sidebar
* Select `Project` then `Add folder to project...` then navigate to folder
* You can remove the folder by right clicking and selecting *remove folder*

#### Multiple Cursors (Helpful for editing more than one line at a time)
* Multiple cursor `alt + ctrl + up/down arrow`
* This feature is a killer one, it makes the transition from a MPC screen to Sublime a little smoother.

#### Add it to the menu
If you'd like to make this quickly accessible from the MPC menu add the following code into 69i2.

```
         MENUBAR,"&SUBLWATCHER"                   
           "&Start watching files",,SUBLWATCHER   
           "&Open report",,SUBL                   
'@'RETURN          
@008:BRK RNM -1 .  
```


## Thanks
A big thanks goes out to John Thalhuber and ITRS for allowing me to use portions of their code in this software.  I'm also very appreciative of the SETUP+ package that he created which allows this application to be installed onto other MAPPER systems with very little friction.  

I'd also like to thank North Star Mutual for allowing me to develop this product.  It's been a joy to be able to build a tool that allows me to get my job done faster with less pain and frustration.  

## Bug Reports
Please report any issues you find with this product in the issues tab in this repository.  I'll do my best to fix issues in a reasonable amount of time, but I get pulled in a lot of directions, and don't always have time to work on this, so be patient if I'm not able to address it very quickly.

## Contributing
If you see features that you would like or want to make something work different feel free to submit pull requests and I'll see if it's something that will fit.  

## Support
At this time Windows 7 is the only OS that's been fully tested.  It was working on XP before switching to Windows 7 and I'm hoping Windows 8 will work out of the box.  If you would like support for other platforms you may have to modify it to work for you.

## License
Portions copyright © IT Resource Solutions (ITRS)
Permission has been granted by ITRS for use of their software in this package.
Copying or reuse of that software is prohibited without the expressed consent of ITRS.

The remaining code is licensed under the MIT license found [here](https://github.com/bis-mapper/sublwatcher/blob/master/LICENSE.md)
