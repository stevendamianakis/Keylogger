# Linux Setup Guide

This guide was implemented on Kali Linux OS, but you can follow it similarly for any Linux OS.


- First, install alacarte with the following command:

```bash
  sudo apt-get -y install alacarte
```

The alacarte module will help us by making the keylogger script as a new application.

- Go to applications > main menu > usual applications > new item > command > python3 path_to_keylogger

For example, if your script is located in Desktop folder then the command will be:

```bash
  python3 /home/user/Desktop/keylogger.py
```

Now, all you need to do, is make the app run on startup.

- Go to Tweaks > Startup Applications > + > name_of_keylogger_app

In some Kali Linux OS versions you will have to make the keylogger run on startup through a different way.
- Go to Session and Startup > Application Autostart > + > fill_out_info_as_before. 

The process of creating the app is the same. This way you will create the keylogger app and configure it to run on startup, at the same time.

The keylogs.txt will be under /home/user because this is the working directory of the keylogger application when it runs on startup.


To terminate the script, open the Task Manager application and search for the script by typing its name "keylogger". Then kill the process by right clicking > kill.
