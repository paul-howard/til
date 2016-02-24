# How to recover voice mails from an iPhone backup in iTunes

## TL;DR

- iTunes > Prefs > Devices; Ctrl-click targeted backup file; select “Show in Finder”
- In terminal, ```cd``` to targeted backup dir (drag Finder proxy icon to auto-fill path in terminal)
- ```> mkdir ~/Desktop/voicemails; for file in `for blah in *; do file $blah; done |grep GSM | cut -f1 -d:` ; do cp -a $file ~/Desktop/voicemails/$file.amr ; done```
- Waaaaaiiit for it…
- All files in the targeted backup identified as Adaptive Multi-Rate Audio (the file format used for voicemails) are now in a folder called “voicemails” on your desktop.

## Source

 [NosillaCast Blog](http://www.podfeet.com/blog/tutorials-5/how-to-recover-your-voicemails-from-an-ios-backup-on-a-mac-for-free/)
