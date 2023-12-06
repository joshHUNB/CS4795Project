Exoplanet Systems:
exoplanet.eu_catalog.csv -(extract unique star names)-> ExoplanetSystems.csv --(only systems with downloadable data)-> FilteredExoplanetSystems.csv --(download Data)-> ExoPlanSystems.txt

Non-exoplanet Systems: 
GaiaDataRaw.csv (renamed from simbad.csv) --(Pull out starNames)-> GaiaStarNames.csv --(stars we have LightCurve data for)-> Gaia_LC_Systems_0_2k.csv --(download Data)-> NonPlanSystems.csv

Multiple versions of Gaia_LC_Systems exist since they took so long to extract. For the final files i generally put the number of star systems at the end, for my main tests I was using ExoPlanSystems500 and NonPlanSystems500. But I couldn't upload them since they were 150-200 MB. Instead i put Example_ExoPlanSystem.txt which has a few data examples to show how the JSON Formatted entries look like. 

If I could I would drastically simplify the number of steps here to weed out the intermediate files. Verify both data sets don't share any stars, then once we know a star has data export it. Would be like 2 csv files for star names then the actual outputs. 
