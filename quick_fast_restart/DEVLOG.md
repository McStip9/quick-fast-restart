Alpha Test

1.0: The program is made.
1.1: Converted batch file to an executable file. (.bat to .exe)
1.2: Added fix when the program doesn't work without making the program elevated.
2.0: Added "This program must be run as administrator".
2.1: Added more text to the new feature.
2.2: Added "=======" for the new feature.
3.0: Added new echo "Please press any key to start..."



Beta Test

4.0: Fixed bug where the program cannot open even if it is run as administrator.
4.1: Fixed bug where the program sometimes shows the log of the "taskkill" command.
5.0: Made quick restart faster, with a whooping 3.4 seconds compared to the 6.7 seconds. Some computers might yield to somewhat faster or slower.
6.0: Added fast_restart.exe.
6.1: Added text file that has all the code of both files.
6.2: Added the batch file version of the files.



CURRENT VERSION: 6.2

==========================================================================================================================
KNOWN BUGS

Accoring to 4.1, it has fixed the big where it sometimes shows the log of the "taskkill" command. However, it still can be seen, even if the bug was fixed.
THIS BUG CAN'T BE FIXED.

Quick restart sometimes take longer than it should. It can be 10.4 seconds (max).
THIS BUG CAN'T BE FIXED. The workaround is to use fast_restart.exe.

You might see a file called "null" after a quick restart of fast restart.
THIS BUG CAN'T BE FIXED.

You might see a large keyboard on your monitor after the quick restart is done. This comes from the "start TabTip.exe". (Note that before the black screen comes there's a code that says "taskkill /f /im TabTip.exe", which is why there's "start TabTip.exe".)
This bug can't be fixed unless you want the "TabTip.exe" removed in the code.

==========================================================================================================================

FEATURES COMING:

