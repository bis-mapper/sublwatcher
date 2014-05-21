
# sublwatcher - BIS file watching utility / IDE environment

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

## SUBLWATCHER - Load application package (File Watching Utility)

1. Download application package [Download](https://github.com/bis-mapper/sublwatcher/archive/master.zip)
2. Unzip file to folder.
3. Sign on as MAPCOORD.
4. Run PCME
5. Click -> Setup -> System Administration
6. Then -> Setup -> Load Application Package
7. Browse to the folder where you unzipped the application package.
8. Open the SETUP.RUN file -> Click Ok
9. The wizard will guide you through the rest of the steps.

## Install Sublime Plugins (Allow Sublime to work with BIS, syntax highlighting, etc)

Follow the commands below to get the syntax files and utilities configured:

* Type `ctrl + shift + p`

* Then `pcar`

* Select *Package Control: Add Repository*

* copy and paste the URL *https://github.com/bis-mapper/bis-sublime* into the input field
at the bottom of the screen.

## Install package

* Type the followinng commands: `ctrl + shift + p`

* Then `pcip`

* Then select *bis-sublime* from the list

* Hit enter

## Plugin repositories
* Refer to [bis-sublime docs](https://github.com/bis-mapper/bis-sublime)
* Refer to [bis-html5  docs](https://github.com/bis-mapper/bis-html5)

# Getting Started

Type `SUBL` on a report that you want to open in BIS.

You will get prompted with a dialog box asking you to find the *sublime_text.exe*.
This should be stored in your program files where you installed Sublime.
Navigate to that folder and select the *sublime_text.exe*

<img src="https://raw.github.com/bis-mapper/sublwatcher/master/Docs/Images/first_time.png" border="0">

## Your file watching folder (sublwatcher)

Some files are downloaded to your workstation when you run the `SUBL` command.  These files are stored in the sublwatcher folder 
`%USERPROFILE% usually c:\users\winne\sublwatcher\`

A browse utility will pop up asking you where you want to put the file that your opening.
<img src="https://raw.github.com/bis-mapper/sublwatcher/master/Docs/Images/browse.png" border="0">

Browse to your sublwatcher folder and select the folder for the site that your currently on.
<img src="https://raw.github.com/bis-mapper/sublwatcher/master/Docs/Images/select_folder.png" border="0">

The BIS report that you typed `SUBL` on will now be saved in this folder and you should be able to modify this file in Sublime and have the changes saved back to BIS.

## Watching Files
You can also type `SUBLWATCHER` on the control line to start the file watching utility.  This skips the process of opening up a specific report and starts the script that watches the files.  This is helpful if you already have the files you want open and just need to start saving the changes back to MAPPER.

## Thanks
A big thanks goes out to John Thalhuber and ITRS for allowing me to use portions of their code in this software.  I'm also very appreciative of the SETUP+ package that he created which allows this application to be installed onto other MAPPER systems with very little friction.  

I'd also like to thank North Star Mutual for allowing me to develop this product.  It's been a joy to be able to build a tool that allows me to get my job done faster with less pain and frustration.  

## Bug Reports
Please report any issues you find with this product in the issues tab in this repository.  I'll do my best to fix issues in a reasonable amount of time, but I get pulled in a lot of directions, and don't always have time to work on this, so be patient if I'm not able to address it very quickly.

## Contributing
If you see features that you would like or want to make something work different feel free to submit pull requests and I'll see if it's something that will fit.  

## Support
At this time I'm only supporting Windows 7.  It was working on XP before switching to Windows 7 and I'm hoping Windows 8 will work out of the box.  If you would like support for other platforms you may have to modify it to work for you.

## License

Portions copyright © IT Resource Solutions (ITRS)
Permission has been granted by ITRS for use of their software in this package.
Copying or reuse of that software is prohibited without the expressed consent of ITRS.

The remaining code is licensed under the MIT license found [here](https://github.com/bis-mapper/sublwatcher/blob/master/LICENSE.md)
