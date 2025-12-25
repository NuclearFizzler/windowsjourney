---
title: Applying GPOs
---
## Applying Group Policy Objects (GPOs)

There's a lot of settings, and it's a waste of time to go through and learn what EVERY SINGLE setting does. Thankfully, people have already gone through and created standard setting templates for you to automatically import.

### Microsoft Security Compliance Toolkit

The [Microsoft Security Compliance Toolkit](https://www.microsoft.com/en-us/download/details.aspx?id=55319) is a set of Windows utilities that allow you to apply Group Policy objects to **Local Group Policies**. (There's another way for Active Directory Group Policies, but we'll discuss them later.)

Included are:
* LGPO.zip / LGPO.exe (Executable that applies the group policies)
* Various Microsoft Security Baselines for different OSes.

The easy thing to do is download your baseline, LGPO.zip, and then apply the baseline policies to your machine.