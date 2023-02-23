# Linux Setup Guide

This guide was implemented on Kali Linux OS, but you can follow it similarly for any Linux OS.


- First, install alacarte with the following command:

```bash
  sudo apt-get -y install alacarte
```

The alacarte module will help us by making the keylogger script run on startup.

- Go to applications > main menu > usual applications > new item > command > python3 path_to_keylogger

For example, if your script is located in Desktop folder then the command will be:

```bash
  python3 /home/user/Desktop/keylogger.py
```

The keylogs.txt will be under /home/user because this is the working directory of the main menu application when it runs the command at startup.


To terminate the script, open the Task Manager application and search for the script by typing its name "keylogger". Then kill the process by right clicking > kill.
