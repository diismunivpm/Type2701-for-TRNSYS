# Type2701-for-TRNSYS
New type for TRNSYS
Type2701 is an extension of the existing type inside the standard library of TRNSYS, capable of simulating a variable capacity 
air-water heat pump for heating.
This model is based on user-supplied data files containing catalog data for the capacity (total capacity in heating mode) and 
Coefficient of Performance (COP).
In particular, given the indications contained in EN 14825:2018, through performance map the model is able to calculate 
the capacity and the COP through interpolation of the performance curve to the variation of the external temperature, 
of the delivery water temperature and of the capacity ratio (CR). Below the minimum modulation CR, the degraded COP is calculated 
according to the indications given within the standard.

At the moment being a preliminary model, the type does not currently take into account the effects due to defrosting.
The Type2701 is OpenSource software under BSD 3-Clause license and anyone can use it and add his contribution to the development;
for details read the file LICENSE.txt.

The repository contains:
-	Type2701 source code (Fortran)
-	dll compiled
-	Batch file of the paths where to insert the folders
-	Data catalog example

For any problem or question please contact:
-	Patricia Ercoli p.ercoli@pm.univpm.it
-	Alice Mugnini a.mugnini@univpm.it
-	Alessia Arteconi a.arteconi@univpm.it