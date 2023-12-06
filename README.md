# CS4795Project

Basic goal for this project was to prototype binary classification of exoplanets. We were able to process data from star names, then using lightKurve (https://docs.lightkurve.org/) downloaded data and fed it into a basif neural network created using Keras functionality. 

Data Sources: Exoplanet positive systems (https://exoplanet.eu/catalog/#downloads-section)
Exoplanet negative systems: https://simbad.cds.unistra.fr/simbad/sim-fout (University of Strasbourg) 

Keep in mind I called many of the inital data processing steps Gaia data X. This is only correct insofar as Gaia data may have been in the simbad's European Space Agency database (since Gaia is an ESA project). I did not use data directly from the Gaia project (https://cdsarc.cds.unistra.fr/viz-bin/cat/J/A+A/649/A6#/browse) (hosted on the same website). 

Main Processing functions are in 'CS4795Project' while the final data download and AI models are in 'CS4795ProjectV2'. 

Program is primarily RAM limited. It was able to run 800 exoplanets on the Google Collab with 12.7 GB available. Running it on full LC data for each system and for all the star systems available would require substantial allocation of RAM.
