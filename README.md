# BCEQ
This repository contains the following:


(A) **ACTUALLY_README.md**
- contains information surrounding data acquisition and analysis methodology

  (1) Colab (Julyter) notebook: [link](https://colab.research.google.com/drive/1DT2BTUE-0tHoaqCcfNEFGPFyZ3caBmhX?usp=sharing)

   -> username: ashley.d.tegart
    -> notebook: EQ_Data_2014_2023.ipynb

   (2) Outside preliminary research sources:

    -> Brogan, Caroline (June 30, 2020). Study reveals how water in deep Earth triggers earthquakes and volcanic activity, Imperial College London, 
      [summary of Cooper et al.’s article]. Retrieved [link](https://www.imperial.ac.uk/news/198796/study-reveals-water-deep-earthtriggers/) 

    -> Cooper, G.F., Macpherson, C.G., Blundy, J.D. et al. Variable water input controls evolution of the Lesser Antilles volcanic arc. Nature 582, 525–529 (2020). [link](https://doi.org/10.1038/s41586-020-2407-5)  


  (3) Code methodology:the code is written in Python with the following python modules

   -> pandas

   -> numpy

    -> matplotlib

   -> ee. (Google Earth Engine) 

   (4) Data sources: see below

   -> all data is publicly available


(B) ****Information About Uploaded Files****: 
 
  (1) **_BC_Coast_EQs.csv**
    
    -> Coastal BC EQ data 2013-2023
   
    -> obtained from from the Natural Resources of Canada Earthquake Database [link](https://www.earthquakescanada.nrcan.gc.ca/stndon/NEDB-BNDS/bulletin-en.php) 
   
    -> the following parameters were used:
      - Start time (UTC): 2013-01-01 00:00:00
      - End time (UTC): 2023-12-31 23:59:59
      - Magnitude from: 3
      - Magnitude to: 10
      - Depth to (km): 0
      - Depth from (km): 100 (although there were no EQs recorded during this time that were over 100km)
      - Minimum latitude: 47
      - Maximum latitude: 62
      - Minimum longitude: -143
      - Maximum longitude: -118
      - Type: quakes
      - Only show felt events: no
      -Format: text
    -> data was uploaded to excel via a csv then uploaded to GitHub
  
  (2) **ERA5 Monthly Aggregates** - Latest Climate Reanalysis Produced by ECMWF / Copernicus Climate Change Service
   
    -> obtained from Google Earth Engine [link](https://developers.google.com/earth-engine/datasets/catalog/ECMWF_ERA5_DAILY)
    -> Dataset availability: 1979-01-02T00:00:00Z–2020-07-09T00:00:00Z
    -> Resolution: 27830 meters
    -> Daily aggregated values for multiple parameters; this research obtained data for 2m air temperature as it included both land and sea surface
      - Band: mean_2m_air_temperature
        - Units: K (kelvin)
        - Minimum: 223.6 "estimated min or max value"
        - Maximum: 220.7 "estimated min or max value"
        - Description: "Average air temperature at 2m height (daily average)"
  
  (3) **_BC_Coast_EQs.xlsx**
    
      -> accidental upload of wrong file type; refused to be deleted
  
  (4) **_EQbook.csv**
      
      -> Early attempt at python with EQ data; refused to be deleted 
