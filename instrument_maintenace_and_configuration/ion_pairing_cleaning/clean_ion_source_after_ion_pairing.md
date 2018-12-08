# Overview

This protocol describes how to clean the ion source after ion-pairing methods (and the ion-pairing dedicated LC) have been used.  

# Equipment

### PPE
Safety glasses and nitrile gloves are required for this protocol.

### For cleaning

* Kimwipes
* 100s of mL of 50% v/v methanol in water (both HPLC grade)
* wash bottle
* sonicator

# Protocol
1. Clean the ion source by following steps 5 - 7 of the [protocol for ion-source cleaning that is part of our biweekly maintenance procedure.](biweekly_maintenance_and_QC.md)
2. Finish cleaning the instrument by doing the 16-hr run of repeated injections and repeated switchings of the LC-MS/waste switching.
	1. Ensure the instrument is set up properly for overnight operation.  Follow the [6470 run start protocol](../start_6470_lcms_run_protocol.md) protocol for help if needed.
	2. Load the `D:\MassHunter\data\mcac\curtf\qc\tea_and_tba_flus.m` method.
	3. Load the `D:\MassHunter\worklists\curtf\qc\tea_flus_300times.wkl` worklist. 
	4. Run the worklist.

# Analysis
To determine the degree to which the cleaning has been effective, `Qual` can be used to monitor the `tributylamine` signal. As an example, here we show the decrease in TBA over the number of cleanings. The cleaning method has a SIM for 186 (TBA) which is plotted below. In purple the first cleaning, in red the 50th cleaning, in blue the 100th, and in green the 150th. Not shown is the ion trace after the 182nd cleaning - it's indistinguishable from the the 150th cleaning run.
![2018/12/08 cleaning](protocols/instrument_maintenace_and_configuration/ion_pairing_cleaning/tba_signal.png)


CF / cf
wdwvt
