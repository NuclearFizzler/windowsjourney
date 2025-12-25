---
title: Local Group Policy
---
## Local Group Policy

Group Policy is the where the "security settings" of Windows are located. These settings control a variety of things from password complexity rules, to what events to log, to whether Windows updates or not. Group Policy overrides settings you configure outside of Group Policy, so if you see the message "these settings are controlled by an Administrator," look in there.

There are 2 big tools to configure Group Policy on individual computers: Local Security Policy, and Local Group Policy Editor.

### Local Security Policy
Access: "Local Security Policy" or `secpol.msc`

Technically, this tool contains a subset of all the Group Policy settings available, but these ones are pretty important.
* Password & Lockout Policy
* Audit Policy
* User Rights Assignment
* Security Options

### Group Policy Editor
Access: "Edit group policy" or `gpedit.msc`

Contains all the Group Policy settings available, including everything in Local Security Policy.

**Computer Configuration vs User Configuration:**
* Computer Configuration - Applied to "computer objects" (settings that work across an entire computer)
* User Configuration - Things applied to individual users

These folders contain different settings and don't overlap!