# Overview

This protocol describes planned biweekly (that means once per two weeks) maintenance procedures on the [ChEM-H MCAC](https://chemh.stanford.edu/knowledge-centers/metabolic-chemistry-analysis-center) LC-MS instruments.

# Equipment
#### PPE
Safety glasses and nitrile gloves are required for this protocol.

#### QC standards
* [*MSRT1 peptide standard*](http://www.sigmaaldrich.com/catalog/product/sigma/msrt1?lang=en&region=US), Sigma Aldrich catalog number `MSRT1`, prepared as specified by manufacturer.
* [*HPLC gradient system diagnostics mix*](http://www.sigmaaldrich.com/catalog/product/supelco/48271?lang=en&region=US),  Sigma Aldrich catalog number `48271`, removed from glass vial and put into HPLC vial.

#### Buffers for cleaning
* 50% v/v methanol (HPLC grade or better) in water (HPLC grade or better)
* 50 &mu;M EDTA (sodium-free) adjusted to pH 7.5 with ammonium hydroxide.
* 70% v/v isopropanol with 30% v/v acetone and 0.1% formic acid for column washing

# Protocol
1. Ensure you have reserved time on the [GNPN ChEM-H LC-MS Schedule](https://calendar.google.com/), a Google Calendar used to reserve time on the instrument.
	* TODO: Link to the specific calendar URL after Lalla creates it.
2. Top off all chromatography buffers.  If needed, make more buffers.
3. Top off all needle wash and pump seal wash "buffers".  If needed, make more working stock of these buffers.
4. Wash an appropriate reversed phase C18 column using our [column-wash protocol](reverse_phase_column_wash_protocol.md).
5. Clean metal ions from the flow path.
	1. If not already available, prepare a solution of 50 &mu;M sodium-free EDTA that has been pH adjusted to a pH of 7.5 with ammonium hydroxide and filtered.
	2. Disconnect the MS from the flow path.
	3. Make three injections of 20 &mu;L of the EDTA solution so that metal ions are removed from the flow path.
	4. Make a 20 &mu;L injection of water to remove EDTA from the flow path.
	5. Hook the MS back into the flow path.
	6. Repeat step 4.
6. Clean spray shields via sonication.
	1. Remove spray shields from the instrument. 
	2. Prepare a beaker of 50% v/v methanol in HPLC-grade water that contains enough volume to cover all spray shields.
	3. Put the solvent beaker containing the spray shields in a sonicator and sonicate for 10 minutes.
	4. Wipe all visible residue from the spray shields with a lint-free cloth or kimwipe. 
	5. If all visible residue is not removed, use 4000 sandpaper to remove remaining residue by abrasion, and repeat step 6.3.
7. Clean the ion source.  
	1. Turn the instrument to standby and allow the ion source to cool.
	2. Open the ion source.
	3. Wet a lint-free cloth or kimwipe with a 50% v/v mixture of methanol and water, and wipe the "left" side of the ion source (i.e. the side that hinges out from the instrument) thoroughly to remove all residue.  If available, use a teflon spray bottle for this step.
	4. Wet a lint-free cloth or kimwipe with a 50% v/v mixture of methanol and water, and wipe the "right" side of the ion source (i.e. the side that is built into the main MS box) thoroughly to remove any residue.  _Never_ use a spray bottle to clean this side of the ion source.  Bulk liquids should never be allowed to enter the MS capillary.
8. As required (frequency TBD) check alignment of the nebulizer probe with the required tools from Agilent. 
	* More info on this step forthcoming.
	* TODO: update protocol with more details here.
9. Replace all spray shields, nebulizers, etc.  Hook up the MS and turn the system on.
10. Run a peptide QC standard and a small molecule QC standard, saving the data in the `D:\MassHunter\data\qc\` folder, using the filename of either `rp_std_<DATE>.d` or `msrt1_std_<DATE>.d` as the filenames.
11. Verify that peak areas and mass spectra for standards meet expectations.
	* TODO: make this step more quantitative.

CF / cf