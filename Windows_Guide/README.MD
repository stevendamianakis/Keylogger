# Windows Setup Guide

This guide was implemented on Windows 10.


- First, save the python script "keylogger.py" and rename it to "keylogger.pyw". This way, whenever the keylogger script is run, it will run in the background and you will not be able to see the terminal popping.

Then, to make the script run on startup, press Windows+R and then type:
```bash
  shell:startup
```

- Add the script, and you are good to go.

To terminate the script, open the Task Manager application and search its name. Then, select the process and hit the “End Task” button to kill the process.

**Warning:** You must add the file, as an exception, in the Microsoft Windows Defender, otherwise the script will be identified as malware.
