# Overview

This protocol describes how to create and execute a worklist to analyze a batch of samples using [ChEM-H's 6470 QQQ mass spectrometer](https://asconfluence.stanford.edu/confluence/display/ICB/ChEM-H+Metabolite+Chemistry+Analysis+Center).  The protocol guides users through the steps of preparation, instrument power-on, calibration, column preparation, and starting an analysis run.  This protocol assumes default choices for chromatography column and ion source.   

# Equipment

### PPE
Safety glasses and nitrile gloves are required for this protocol.

### Samples
Your samples must be prepared for LC-MS analysis.  
* All samples must be filtered using 0.45 &mu;m or 0.22 &mu;m filters.  Avoid freezing your samples after filtering.
* Your samples must be in either HPLC vials or 96-well plates.  The containers for your samples must be compatible with organic solvents such as methanol or acetonitrile.  This most commonly means that glass vials or polypropylene plastics must be used.  Avoid polystyrene and similar materials.
* The minimum volume of each sample depends on the container type.

### Instrumentation
#### Chromatography column
This protocol assumes users will be using our standard reversed-phase chromatography setup.  Our default choice is a [50 mm &times; 2.1 mm Zorbax RRHD Eclipse C18 column with 1.8 &mu;m beads (Agilent #959757-902)](http://www.agilent.com/store/en_US/Prod-959757-902/959757-902).  The column should be fresh or recently cleaned.  See [protocols](instrument_maintenace_and_configuration/reverse_phase_column_wash_protocol.md) on cleanup of reverse-phase chromatography columns for more information.


### Reagents
#### Calibrants and standards
* Reference bottle A  
* Tuning Mix bottle B
Both of these bottles housed in the LC-MS itself should be full. See [this document](tuning_mix.pdf) for information on the composition of the tuning mix.
* [HPLC gradient system diagnostics mix (Aldrich #48271)](http://www.sigmaaldrich.com/catalog/product/supelco/48271?lang=en&region=US).  This should usually be present in the `Vial 1` position inside the autosampler.

#### Chromatography "buffers"
* Line A: HPLC-grade water containing 0.1% v/v formic acid.
* Line B: HPLC-grade acetonitrile containing 0.1% v/v formic acid.
* Needle wash / pump head wash: 15% v/v HPLC-grade isopropanol in HPLC grade water

Each bottle should contain more than 300 mLs of buffer.

### Worklist

Prepare a worklist for your samples using Microsoft Excel or Google Sheets or a similar program.  The spreadsheet you use should contain the following columns:

| Sample Name | Sample Position | Method | Data File | Inj Vol (&mu;L) | 
|-------------|-----------------|--------|-----------|-----------------|
| my_fav_samp | P1-A1           |my_meth.m| my_fav.d | 1               |
| 002         | P1-A2           |my_meth.m| 002.d    | 1               |
| condition_B_again | P1-A3     |my_meth.m| B_again.d| 1               |
| ...| ...    |...| ...| ...               |


We recommend that the first injection -- and approximately every 20th injection you make -- be of [HPLC gradient system diagnostics mix (Aldrich #48271)](http://www.sigmaaldrich.com/catalog/product/supelco/48271?lang=en&region=US).  

We also recommend that you randomize injection order for your samples.


# Protocol
1. Ensure you have reserved time on the [GNPN ChEM-H LC-MS Schedule](https://calendar.google.com/calendar?cid=M2VpYzByOGM2am10ZGY5ZTM1MGRnOGNsNzRAZ3JvdXAuY2FsZW5kYXIuZ29vZ2xlLmNvbQ), a Google Calendar used to reserve time on the instrument.
2. Ensure the instrument is prepared for your run.
	1. Ensure that all required equipment, including (filtered) samples, the appropriate chromatography column, the proper ion source, calibrants, and chromatography buffers and needle washes, are present.  
	2. Ensure that waste containers are not full.
	3. Ensure that nitrogen sources to the instrument are adequately pressurized.  The nitrogen generator should be putting out &approx; 100 psig of nitrogen, and the UHP nitrogen behind the door should be putting out 20 psig.
3. Put your samples in the autosampler.  If needed, move old samples from previous users to the "Old Samples -- Will Be Discarded Soon" shelf.
4. Open MassHunter Workstation Data Acquisition software if it is not already open.
5. Begin filling out the required log sheet.  Enter your SUNET ID, sample types, column type and location. Check off the box for completing instrument inspection.
6. Open your analysis method.  It should use a chromatographic flow rate of 0.6 mL / min.
7. Let the ion source, column oven, and other components warm up.  Wait until the indicator for each component turns GREEN.
9. Set up your Worklist.
	1. Set the default file paths for methods and data in `Worklist Run Parameters`.  
	2. Show/hide the columns in the Worklist view to match the columns in the sample Worklist shown above.
	3. Copy and paste from Excel to Acquisition.
	4. Add the `InstrumentStandby` script to the end of your worklist.  Check off the space on the log sheet to indicate that you have done so.  
		* This prevents endless pumping of chromatography buffer, dried pumpheads, overflowing waste containers, etc.
	5. Save your worklist.
10. Ensure the autosampler plate types are set correctly.  Right click on the autosampler module, select "Assign Wellplates".  Make sure the plate types defined in the software match the plate types in the autosampler.
11. Check the details of your data acquisition methods one last time.  
	* Are you diverting the first few column volumes to waste?  This is a good idea if you have "dirty" samples.
	* Are your MS and MS/MS acquisition parameters set correctly?
12. Click the "Start Worklist Run" button.
13. Watch the first sample inject to be sure no errors occur.
14. Observe the TIC plot data in the Acquisition window to make sure the peaks in the first injection (of the external standard) look correct.
15. You are free to leave and let the instrument do its work.  It's a good idea to check in on your run periodically using AnyDesk.
16. If you want your samples back, retrieve them from the autosampler before your reserved time on the calendar ends.

CF / cf
