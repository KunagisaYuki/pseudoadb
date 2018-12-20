# Features configure

This doc describe configure file properities.  
These information should be written into /sdcard/.pseudoadb/features.conf
If some of these properities are not set , they will set to the default value of 1 (Some exeception are marked out).

## Current available properities

## In progress

### adb_install = {0,1,2}

- 0：Disable installation hook
- 1: Enable installation hook (Deny all installation , return false fail)
- 2: Enable installation hook (Accept installation , install sandbox packed application)

### adb_applist = {0,1}

- 0: Disable applist hook
- 1: Use /sdcard/.pseudoadb/applist.conf to provide fake list

### filesystem = {0,1}

- 0: Disable filesystem hook
- 1: Use /sdcard/.pseudoadb/fs to provide fake list

### shell_honeypot = {0,1,"strings_to_honeypot_shell"}

- O: Disable shell hijack
- 1: Use inbuilt fake shell.
- "strings_to_honeypot_shell": Use custom binary provided by the string.
