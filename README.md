# Milkyway-7-21 allows BOINC to obtain new work from Milkyway constantly
Please use Word and read the docx to see how the build is done
If you are running my 7.16.3 mod then substitute my mod for the 7.16.3 mod as follows
Exit boinc manager and allow it to stop all jobs.  Verify BOINC.EXE is not running
using the device manager.  Terminate the app if it is still running.
Bring up an administrators command windows and change folder to c:\program file\boinc
rename boinc.exe to boinc-7-16-3
rename boinc-7-21.exe to boinc.exe and verify it works using "boinc.exe --version"
Start boinc manager and bring up the event log and verify 7.21 is running.
I no longer have 7.15 on any systems but I assume 7.21 can be substituted for it
You might want to backup the contents of boinc in the event you want to restore
7.15 or 7.16.3
Version 7.21 only has a mod for the Milkywsay work fetch bug and does not have the 
features of 7.16.3
