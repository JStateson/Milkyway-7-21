# Milkyway-7-21 allows BOINC to obtain new work from Milkyway constantly

If you are running 7.15 Windows or Linux there is no Milkyway benefit to 7.21 unless you want the functionality of 7.20.  If so then uninstall 7.15 and install 7.20 before using the mod.  This applies to both the Windows and Linux versions.

Please use Word and read the docx to see how the build is done ONLY IF YOU WANT TO BUILD IT

The Linux version can also be built as documented, or you can download the tar file AFTER reading the doc

If you are running my 7.16.3 mod then substitute this mod for the 7.16.3 mod as follows

Exit boinc manager and allow it to stop all jobs.  Verify BOINC.EXE is not running

using the device manager.  Terminate the app if it is still running.

Bring up an administrators command windows and change folder to c:\program file\boinc

rename boinc.exe to boinc-7-16-3

rename boinc-7-21.exe to boinc.exe and verify it works using "boinc.exe --version"

Start boinc manager and bring up the event log and verify 7.21 is running.

I no longer have 7.15 on any systems but I suspect it must be uninstalled.

You might want to backup the contents of boinc in the event you want to restore 7.15, 7.16.3 or 7.20.2

Version 7.21 only has a mod for the Milkyway work fetch bug and does not have the features of mod 7.16.3

This app WILL NOT FUNCTION PROPERLY if Milkyway CPU apps are run along with GPU apps.
Run CPU apps such as WCG or Universe.  I am not interested in fixing the CPU app problem.

Make sure you have at least 0.25 day of "additional" wanted work

Please read the filter_readme file for before downloading any of the filter files.