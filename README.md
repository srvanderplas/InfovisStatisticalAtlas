# InfovisStatisticalAtlas
2017 InfoVis paper - Reproducing plates #31 and #32 of the 1870 Statistical Atlas


# Files and Folders
- scripts: Conversion scripts from raw data to useable aggregated data
    - 01_ipums-ages.R:    
    This script will not run without additional data which cannot be released due to IPUMS licensing restrictions.
    - 02_occupation-to-occ2.R:    
    Creates the occ2.csv data file. Aggregates state-level occupation information from the 1% microsample.
    - 03_ages-to-occ3.R:    
    Aggregates occupations by age and gender using estimation formulas. 
    - 04_to-px2.R:    
    Reads raw pixel values and converts that information into population numbers and percentages.
    - 05_tot10-to-denom.R:    
    Creates the denominations data frame out of the ipums census microsample.
    - 06-pix-tounaccommodated-plate31.R:    
    Reads raw pixel values and converts that information into population numbers and percentages.

- Data-raw: Raw data files - 1870 census aggregates and pixel value measurements
    - church_accomodations-w-percent-unacomodated-area.csv:    
    Measured pixel values for plate #31 of the statistical atlas
    - denominations-1874.csv:    
    Population numbers and percentages for church accomodation as measured from the 1% microsample of the 1870 US Census
    - occupation.csv:    
    Aggregated information from the 1% microsample of the 1870 US Census
    - pixel-values.csv:    
    Measured pixel values for plate #32 of the statistical atlas
    - state-population.csv:    
    State populations according to the 1870 census.
- Data
    - ages-ipums.csv:    
    Population estimates by age for the 1870 census.
    - ages-sex-ipums.csv:    
    Population estimates by age and sex for the 1870 census.
    - church_pixel.csv:    
    Estimates from the statistical atlas for church accomodation
    - denominations-1874.csv:    
    Estimates from the 1870 US Census for denominations by state
    - occ2.csv:    
    Estimates of population in each occupation by state and gender
    - occ3.csv:    
    Estimates of population in each occupation by state, age, and gender, including unaccounted population.
    - px2.csv:    
    Pixel measurements from plate #32.
