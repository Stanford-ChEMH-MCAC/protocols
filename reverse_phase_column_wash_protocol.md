# Overview

This protocol describes how to wash a contaminated or plugged reverse-phase HPLC column with aggressive, hydrophobic solvents in attempt to clean it and lower pressure drops.  It is specific for  [ChEM-H's 6545 Q-TOF mass spectrometer](https://asconfluence.stanford.edu/confluence/display/ICB/ChEM-H+Metabolite+Chemistry+Analysis+Center).

# Equipment
#### Chromatography column

This protocol assumes the column to be washed is a [50 mm &times; 2.1 mm Zorbax RRHD Eclipse C18 column with 1.8 &mu;m beads (Agilent #959757-902)](http://www.agilent.com/store/en_US/Prod-959757-902/959757-902).  

#### Chromatography "buffers"
* Line A1: HPLC-grade water containing 0.1% v/v formic acid, e.g. []().
* Line B1: HPLC-grade acetonitrile containing 0.1% v/v formic acid.
* **Line A2: 70% v/v isopropanol, 30% v/v acetone, 0.1% v/v formic acid by volume**.  
	This is the main wash solvent used. 
* Needle wash / pump head wash: 15% v/v HPLC-grade isopropanol in HPLC grade water

Each bottle should contain more than 300 mLs of buffer.


# Protocol
1. Ensure you have reserved time on the [GNPN ChEM-H LC-MS Schedule](https://calendar.google.com/calendar/ical/gnpn.chemh.lc.ms%40gmail.com/private-0590e5f4df42c4d33d6fbb8ab1d0bb40/basic.ics), a Google Calendar used to reserve time on the instrument.
2. Ensure the instrument is prepared for washing your column.
	1. Ensure that required chromatography buffers are present.
	2. Ensure that waste containers are not full.
3. Open MassHunter Workstation Data Acquisition software if it is not already open.
4. Open a representative analysis method.  It should use a chromatographic flow rate of 0.6 mL / min.
5. Let the column oven, and other system components warm up.  Wait until the indicator for the column oven turns GREEN.  It is not necessary to wait the mass spec to warm up.
6. Turn off the binary pump or set the flow rate to 0 mL / min.
7. Connect the column to be cleaned in reverse orientation.
	1. Open the column oven.
	2. Disconnect the existing column.
	3. Connect the column to be cleaned in reverse orientation.  
		To do so, tighten the fingertight connectors until you first feel a slight resistance, and then tighten the column switch.
		The purpose of connecting the column in the reverse orientation is so that dirty end (i.e. the usual "top" of the column) is nearest to the _exit_, so that contaminants do not have to traverse the whole column to be cleaned.
	4. Close the column oven.
8. Flow at least 20 column volumes of acetone/IPA over the column.
	1. Select buffer `A2` as the `A` line buffer.
	2. Purge the pump to clear residual `A1` buffer from the `A` line.  (Right-click on the pump module, select `Prepare Pump`, and flow 100% buffer A at 5 mL / minute for 2 minutes.)  
	3. After purge is complete, the pump status will change from yellow to green.  Let at least 20 column volumes of buffer A2 flow over the column.  
9. Flow at least 40 column volumes of acetonitrile over the column and purge all acetone/IPA from the lines.
	1. Stop the pump flow.
	2. Select buffer `A1` as the `A` line buffer.
	3. Purge the pump to clear residual `A2` buffer from the `A`, as described above.
	4. After purging, change the solvent flow to the pump to 100% buffer `B1`, i.e. 100% acetonitrile with 0.1% v/v formic acid.
	5. Let 40 column volumes of acetonitrile flow over the column.
	6. Ensure that system pressure and UV absorbance stabilize at this condition.  Acetone absorbs strongly at 254 nm and thus as acetone is removed from the column UV absorbance will drop over time.  Make sure this drop is complete and UV baselines have stabilized.
10. Open the column oven.  Disconnect the column and connect it in the **correct* flow direction.
11. Set the flow to the column to correspond to your initial method conditions (e.g. 95% buffer `A1`, 5% buffer `B1`) and let 40 column volumes of this mixture flow over the column.
12. If you are using the column immediately, you are ready to begin your run.
13. If you are storing the column for later use, store it in 100% acetonitrile.
	1. Change the buffer to 100% buffer `B1`. 
	2. Flow at least 10 column volumes of buffer `B1` over the column.
	3. Stop the pump, set the instrument to standby, disconnect the column, plug the ends with stoppers, and store at room temperature.
	
CF / cf
