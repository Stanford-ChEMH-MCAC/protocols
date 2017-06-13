# Overview

This protocol describes how to safely power cycle the 6545 qTOF mass spectrometer.  It is useful for when communications between the MS and its controlling PC break down, or when the mass spectrometer is generating cryptic, non-sensical error messages.

# Equipment

# Protocol
1. Ensure you have reserved time on the appropriate ChEM-H LC-MS schedule:
	* The Agilent 6545 QTOF calendar is at [GNPN ChEM-H LC-MS Schedule](https://calendar.google.com/calendar/embed?src=gnpn.chemh.lc.ms%40gmail.com&ctz=America/Los_Angeles)
	* The Agilent 6470 QQQ calendar is at [QQQ_6470](https://calendar.google.com/calendar/embed?src=3eic0r8c6jmtdf9e350dg8cl74%40group.calendar.google.com&ctz=America/Los_Angeles)
 
2. Close MassHunter
3. Click the "Remove MassHunter Processes" icon on the desktop.
4. Click the Shutdown Smart Card logo.
5. Click the "shutdown" button in the popup window.
6. Read the scary dialog box that comes up and heed its instructions.
7. Click "OK".
8. After the PC tells you that the instrument *must* be power cycled, it is safe to do so:
9. Turn off the power switch at the lower left corner of the front of the instrument **FOR NO MORE THAN 5 SECONDS**.
10. After **NO MORE THAN 5 SECONDS**, turn the instrument back on.
11. After you have turned the instrument back on, make sure the rough pump (the big metal thing on the floor) is running.
12. Restart the MassHunter computer and wait ~ 5 minutes for the MS to stabilize.
13. When the computer restarts, log back in and click "the Q-TOF diagnostic Tool" logo on the desktop.
14. When that tool opens, click the "Connection" menu and choose "Connect".  Accept the default IP address.
15. You might have to wait awhile for the MS to connect.
16. Once the software gives up connecting, click "Recover Fault"
17. Repeat step 13.  The "Connection" logo on the bottom right of the window should turn green.
18. If so, you're in business.  Close the "Q-TOF diagnostic Tool" software.
19. Start MassHunter and enjoy your life as a mass spectrometrist!

CF / cf
