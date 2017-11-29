# Overview

This protocol describes how to change chromatography buffers on ChEM-H's LC-MS instruments.  This protocol is useful when you have reserved instrument time, and need to exchange the buffers currently plumbed to the instrument to new buffers suitable for your chosen analysis method.

# Equipment
#### PPE
Safety glasses and nitrile gloves are required for this protocol.

#### Buffers
* Buffer "C" and "D" of your choosing should be available.  **You will be installing these buffers on lines *C* (or *A2*) and *D* (or *B2*) of the instrument**, as lines A(1) and B(1) on both of our instruments are dedicated to water and acetonitrile respectively, both with 0.1% v/v formic acid.  

* On the 6545 qTOF, there is no line "C" or "D"; instead, these lines are called "A2" and "B2".  Lines A1 and B1 are dedicated to water and acetonitrile.

Only use buffers made from HPLC-grade solvents, and make sure the solvent strength and pH of your buffer is compatible with your column.

#### Other
* two small beakers (<= 250 mL capacity)
* Kimwipes or other lint-free towelettes

# Protocol
1. Ensure you have reserved time on the appropriate ChEM-H LC-MS schedule:
	* The Agilent 6545 QTOF calendar is at [GNPN ChEM-H LC-MS Schedule](https://calendar.google.com/calendar/embed?src=gnpn.chemh.lc.ms%40gmail.com&ctz=America/Los_Angeles)
	* The Agilent 6470 QQQ calendar is at [QQQ_6470](https://calendar.google.com/calendar/embed?src=3eic0r8c6jmtdf9e350dg8cl74%40group.calendar.google.com&ctz=America/Los_Angeles)
2. Open the bottles of the new buffers that you will add to the system.  This protocol assumes that you have two such buffers, which we will call C & D.  
3. Rinse one beaker 2&times; with a small amount of new buffer C.  Dispose of the wash in the LC-MS waste bottle.  Rinse the other beaker 2&times; with a small amount of new buffer D.  Dispose of the waste similarly.
4. Label the beakers.  Fill one beaker with ~50 mL of buffer C, and with ~50 mL of buffer D.
5. Remove the cap and solvent inlet filter from the old, to-be-replaced buffer C.  Dry the solvent inlet filter with a kimwipe.
6. Dip the line C solvent inlet filter into the beaker filled with buffer C and hold it so it is submerged.
	* CAUTION: is easy to accidentally tip over the beaker during this step; do not try to prop the C-line bottle cap and solvent inlet filter agains the side of the beaker.  Hold it at all times.
7. Purge line A for ~30 seconds at 2.5 mL/min.
	* This step avoids contamination of your large bottles of new buffer with any trace amounts of the old buffer that adhere on and in the solvent inlet filter, but it is insufficient to completely remove all of the previous buffer from the tubing that feeds the pump.
8. Stop the pump, remove the solvent inlet filter, and blot it dry with a kimwipe.  Dispose of the contents of the beaker into the LC-MS waste container.
9. Insert the dried line C bottle cap / solvent inlet filter into your bulk bottle of new buffer A and tighten the lid.  Make sure the solvent inlet filter rests on the bottom of your new bottle of buffer.
10. Repeat steps 5-10 with line D instead of line C.
11. Purge both buffer lines at a flow rate of 2.5 mL / min for at least 5 minutes.
	* You can accomplish this step by purging both lines simultaneously at a flow rate of 5 mL/min and a solvent blend of 50% C, 50% D (or 50% A2 / 50% B2).
	* This step purges the bulk of the old buffer from the lines.
12. Find dry lids to put on the old bottles of buffer C and D that you have removed from the system, and store the old buffers in an appropriate place.
13. **Important**.  Right click on the pump module, select "Bottle Fillings...", and update the pump's solvent volume tracker with volumes and bottle sizes for your new buffers.

CF/cf