# MacOS Setup Guide

This guide was implemented on MacOS Monterey 12.4

- First, open the Automator app, which is pre-installed in MacOS.

- Go to Application > Run Shell Script (drag it to the right side) > Pick a shell type(/bin/zsh in my case)

Now, enter the following script in the bash script:

```bash
  #!/bin/Shell
  
  killall ScriptMonitor

  python_executable_path keylogger_path
```
> python_executable_path = the path of the executable file of python

> keylogger_path = the path of your keylogger script

In my MacOS, python was installed using Homebrew, so the python_executable_path was "/usr/local/bin/python3". If you have not installed python using Homebrew, then check for your correct python executable path. 

So my final script was:

```bash
  #!/bin/Shell
  
  killall ScriptMonitor

  /usr/local/bin/python3 /Users/user/Desktop/keylogger/keylogger.py
```

The "killall ScriptMonitor" command will ensure that the keylogger script gear icon from Automator, will not be visible in the main menu bar. You can remove the command if you want to see the gear icon.

- Save the script under the Applications folder. In this case, the name was "keylogger_app".

- Next, give permission to the python keylogger script and the keylogger app, for "Input Monitoring" and "Files and Folders". 

- Go to Apple Logo > System Preferences > Security & Privacy > Input Monitoring (add the app and the script)

- Go to Apple Logo > System Preferences > Security & Privacy > Accessibility (add the app)

- Double click the keylogger app and allow access to files and folders.

- To make the app run on startup, go to Apple Logo > System Preferences > Users and Groups > Login Items > keylogger_app (add the app)

The keylogs.txt will be under /Users/user because this is the working directory of the application when it runs at startup.


To terminate the script, open the Activity Monitor application and search for the script by typing its name "keylogger_app". Then kill the process by double clicking > quit.

**Warning:** In MacOS, there is a feature called "Secure Keyboard Input". It is a feature on MacOS that prevents apps from intercepting key events sent to other apps when typing in private information, like passwords. Our keylogger app will be able to record passwords, only from a small percentage of websites.
