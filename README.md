# Type2701-for-TRNSYS
Type2701 version 1.0 is an extension of the existing type inside the standard library of TRNSYS (TRNSYS 17, 2014), capable of simulating a variable capacity air-water heat pump for heating.
This model is based on user-supplied data files containing catalog data for the capacity (total capacity in heating mode) and Coefficient of Performance (COP).
In particular, given the indications contained in EN 14825:2018 (CEN, 2018), through performance map the model is able to calculate the capacity and the COP through interpolation of the performance curve to the variation of the external temperature, of the delivery water temperature and of the capacity ratio (CR). Below the minimum modulation CR, the degraded COP is calculated according to the indications given within the standard.
As sample catalog data an air-water heat pump from Viessman was taken (Viessmann, 2020).

At the moment being a preliminary model, the type does not currently take into account the effects due to defrosting.
The Type2701 is OpenSource software under BSD 3-Clause license and anyone can use it and add his contribution to the development; for details read the file LICENSE.txt.

The repository contains:
-	Type2701 source code in Fortran ("Type2701.f90" file in "DLL compiled")
-	DLL compiled
-	Batch file of the paths where to insert folders and files
-	Sample catalog data

For any problem or question please contact:
-	Patricia Ercoli p.ercoli@pm.univpm.it
-	Alice Mugnini a.mugnini@univpm.it
-	Alessia Arteconi a.arteconi@univpm.it

Example of application:
-Hybrid Heat Pump Systems: Is Predictive Control Worth Using?
Ercoli, P., Mugnini, A., Polonara, F., Arteconi, A.
Proceedings of Building Simulation Applications, 2022, pp. 25–32.
 https://publications.ibpsa.org/conference/paper/?id=bsa2022_9788860461919_04

References:
- CEN (European Committee for Standardization), Standard EN 14825:2018. 2018. Air Conditioners, Liquid Chilling Packages and Heat Pumps, with Electrically Driven Compressors, for Space Heating and Cooling – Testing and Rating at Part Load Conditions and Calculation of Seasonal Performance
- TRNSYS 17 - Transient System Simulation Tool. 2014. Version 17.2, Solar Energy Laboratory, University of Wisconsin, Madison, USA.
- Viessmann. 2020. “VITOCAL 250-S: Air-to-water heat pump for hybrid operation 1.1 - 13.4 kW” commercial datasheet.
