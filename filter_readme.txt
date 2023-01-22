All the files in this github repository require that you have first installed
BOINC version 7-20.  Possily the executable may work with older or newer BOINC
apps but I cannot guarantee that.

These executables and files name with "filter_7_21" remove message clutter to
make it easier to find more important messages in the BOINC 7.20 app's event file.
If you are running BOINC on only one system, you probably have no need to reduce
the number of messages.

gui_rpc_server_ops.cpp

This file had 3 lines of code commented out.  The lines of code informed the user
that Works Units had been suspended, resumed, or aborted.  Note that the user
must have caused this to happen in the first place so the message are not very
informative. If you are dealing with 100s of work units, the event log quickly gets
overrun and important message are either hidden or removed. Note also that these
messages originate from the app and not from the server.

cs_scheduler.cpp

In addition to the "fix" to allow Milkyway to constantly acquire more work units,
the file was edited to
 (1) Prevent low priority messages from being displayed.
 (2) Allow the user to specify which messages from the server are to be ignored
     Note that this affects only message form the server, not the app or the user.

MsgExcludedList.cfg

This config file allows the user to specify custom messages filters to prevent the
server from spewing a lot of unnecessary or unwanted information into the event logs.
Place this file into \ProgramData\Boinc or /var/lib/boinc 
This file is only used by cs_scheduler.cpp.  If the file is not found, then no server
filtering is done.  gui_rpc_server_ops does not use this file so it will continue to
remove those user messages.  You must re-start BOINC after editing, adding, or
removing this config file.

