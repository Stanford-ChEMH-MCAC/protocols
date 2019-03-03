# Overview

This protocol describes how to derivatize samples containing ketones or aldehydes with Girard's T reagent for improved LC-MS analysis. 

# Equipment

### PPE
Safety glasses and nitrile gloves are required for this protocol.

### Samples

Samples for this protocol are assumed to be already-extracted, clarified liquids.  They might be [plant tissue extracts](general_metabolite_extraction_from_plant_tissue.md) or [filtered microbial culture supernatants](ht_sample_filtration_protocol.md), or any sample that is suitable for injection on a C18 chromatography column and LC-MS system.

* Thus, samples cannot contain particulates, precipitates surfactants, or high concentrations of non-volatile salts.


### Reagents

1. [Girard's T reagent](https://www.sigmaaldrich.com/catalog/product/sial/89397?lang=en&region=US), e.g. Aldrich catalog # `89397`.

2. [Glacial acetic acid](https://www.fishersci.com/shop/products/acetic-acid-glacial-hplc-fisher-chemical/A35500), e.g. Fisher catalog #`A35-500`

3. LC-MS-grade methanol

4. Suitable vials and vial closures (lids) for holding samples dissolved in organic and aqueous samples and for LC-MS injection.


# Protocol

1. Prepare stock solution of T reagent.
	1. weight 20 mg of Girard's T reagent into an LC-MS vial or similar container.
	2. Add 1 mL of HPLC-grade methanol.
	3. Mix until completely dissolved.
		* This stock solution is not shelf stable for long periods and is best prepared fresh before use.

2. Mix 100 &mu;L of each sample with 100 &mu;L of Girard T stock solution in an LC-MS vial.
	* LC-MS 96-well plates are perhaps compatible with this protocol: it may be difficult to seal the plate tightly during the heating step below.  Without a tight seal, solvent will evaporate in an uncontrolled way during derivatization.  Test your equipment before use on precious samples.

3. Add 20 &mu;L of glacial acetic acid.

4. Incubate samples at 70 &deg;C for 1 hr.

5. Let samples cool to near room temperature.  They are now ready to inject.

# Chemistry

The Girard's T reagent:

* is (carboxymethyl)trimethylammonium chloride hydrazide
* has CAS number of 123-46-6 
* has a PubChem CID of [67156](https://pubchem.ncbi.nlm.nih.gov/compound/67156)
* has a SMILES structure of `C[N+](C)(C)CC(=O)NN.[Cl-]`
* is detectable (in unreacted form and if present in excess or unreacted with carbonyls) at an $m/z$ of 132.1131 .
	* also shows a prominent ion corresponding to (M+ - H2O - N2)+, i.e. C5H11N+, at $m/z$ of 86.0964 .
* replaces the carbonyl oxygen with a hydrazone moiety.
* A SMARTS reaction model for the derivatization might be `[#6:3]-[C:1]=[O:2]>>[#6:3]-[C:1]=NNC(=O)C[N+](C)(C)(C)`
* increases the _exact mass_ of derivatized analytes by 114.1026 Da and the charge of analytes by +1. 
* increases the _measured m/z_ of derivatized analytes by 113.0953 Da.
* was first described in 1936 by [Andre Girard & Georges Sandulesco](http://dx.doi.org/10.1002/hlca.193601901148) in Helvetica Chimica Acta (in French).

# Acknowledgements

Ryan Nett contributed to this protocol.

CF & RN / cf
	

