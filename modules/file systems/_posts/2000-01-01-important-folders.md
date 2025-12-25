---
title: Important Folders
---
## Important Folders

### PATH and System Folders

The PATH variable is a variable telling your operating system where to "look"
for binary applications. For example on Linux, the "ls" command is an executable program in `/usr/bin/ls`. In fact, a lot of commands are located in the `/usr/bin` folder; thus, that folder is in PATH.

An equivalent folder to `/usr/bin` is the infamous `C:\Windows\System32`. It contains Windows utilities like `cmd.exe` and Task Manager, Windows Logs, and a variety of other important system-related stuff. In short, if someone messes with this folder, you're going to have a bad day.

Why bring this up? Well, when you open a utility from the Start Menu, it's looking for a name match in the System32 folder. For example, when you run Task Manager, it's actually calling the program `C:\Windows\System32\Taskmgr.exe`. If you were to swap the names of programs, Windows wouldn't know any better.

### Example of Red Team Persistence

Here's a classic example. You probably know of Sticky keys - hit SHIFT 5 times and you'll hear the funny beep with a menu. It's actually calling a certain executable in System32. Now, say we were to replace that executable with a renamed `cmd.exe`. If someone activated Sticky Keys, they would instantly have a shell.

Did you know Sticky Keys works on the login screen, even when you haven't logged in yet?

Reference: <https://docs.datadoghq.com/security/default_rules/def-000-a8k/>
