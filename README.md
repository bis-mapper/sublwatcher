
# sublwatcher - BIS file watching utility / IDE environment

<img src="https://raw.github.com/bis-mapper/sublwatcher/docs/images/master/sublwatcher.png" border="0">

## Initial Requirements

In order to use this you must first install Sublime Text and Package Control.

[Sublime Text](http://www.sublimetext.com/3)

[Package Control](https://sublime.wbond.net/installation)

## Dependencies

Python 2.7

[Python Download](http://www.python.org/ftp/python/2.7/python-2.7.amd64.msi)

* Download [Distibute Setup](http://python-distribute.org/distribute_setup.py)
* `cd c:\python27\`
* Now run `c:\python27\distribute_setup.py`
* Install *pip* `c:\python27\scripts\easy_install.exe pip`
* Install *watchdog* `c:\python27\scripts\pip install watchdog`

Install Growl for Windows

[Growl Download](http://www.growlforwindows.com/gfw/d.ashx?f=GrowlInstaller.exe)

* Follow setup instructions
* Once installed open up the growl GUI interface (System Icon tray in windows)
* You can set your defautl Displays and check to start program when computer is booted)

## sublwatcher - install in BIS

* Download the repository to your workstation [Sublwatcher Download](https://github.com/bis-mapper/bis-sublime/archive/master.zip)
* Unzip the files
* APPLOAD the purge file to cabinet of your choosing (I have mine in 56)
* REGISTER the following runs in your development dept
    * `SUBL` - `2B56` or substitue your cabinet
    * `SUBLWATCHER` - `3B56` or substitue your cabinet

## Install Sublime Packages (Syntax files and utilities)

* Refer to [bis-sublime docs](https://github.com/bis-mapper/bis-sublime)
* Refer to [bis-html5  docs](https://github.com/bis-mapper/bis-html5)



# Getting Started

To start using for the first time go to a BIS report that you want to open in Sublime.
You will get prompted with a dialog box asking you to find the *sublime_text.exe*.
This should be stored in your program files where you installed Sublime.  Navigate to that folder
and select the *sublime_text.exe*

<img src="https://raw.github.com/bis-mapper/sublwatcher/docs/images/master/sublwatcher.png" border="0">

## Your file watching folder (sublwatcher)

Some files are downloaded to your workstation when you run `SUBL` command.  It also creates a folder in your %USERPROFILE% (usually c:\users\winne\sublwatcher\)

A browse utility will pop up asking you where you want to put the file that your opening.
<img src="https://raw.github.com/bis-mapper/sublwatcher/docs/images/master/browse.png" border="0">

Browse to your sublwatcher folder and select the folder for the site that your currently on.
<img src="https://raw.github.com/bis-mapper/sublwatcher/docs/images/master/select_folder.png" border="0">

A file will now be stored in that folder and opened up in Sublime.

