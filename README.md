# pseudoadb

A fake adb to use as honeypot

## why

Some of you have heard about the phone scanning in some Chinese cities. This tool will prevent such check by fake adb result.

## current target

- log commands
- provide fake system info
- give pseudo shell
- provide fake package list
- stop application installation
  - stop installation
  - pack the application into a sandboxed one.

## How to use

### For End Users

//Todo: add magisk download entry  
Download the binary from our CI then install it via magisk.  
We're going to have an app to configure it's feature, Currently we use /sdcard/.pseudoadb/features.conf  
See [features_conf](docs/features_conf.md)

### For Developers

Copy these files into normal adb code then compile it.  
If you need these supportive binaries, use make buildbinaries
