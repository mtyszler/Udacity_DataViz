# Links to the Tableau Public workbooks
Version 1: 
https://public.tableau.com/views/HDR_v1/HDIStory?:embed=y&:display_count=yes&publish=yes



# Summary
This visualization shows the progress of the Human Development Index over time. The focus is on the fact that while World average has increased, and most countries increased their own HDI, the gap (i.e. difference) between regions remains. In particular, Africa is constantly at the bottom and Europe constantly at the top for the HDI and its 3 components.


# Design
I opted to have the Tableau Story told in 4 steps: 
* Step 1: World averages
* Step 2: Break down by Region
* Step 3: Evolution, by Region, of the 3 components
* Step 4: Break down by Country, within region

For all visualizations I opted to highlight the limit point above which it is considered (at least) medium human development (0.550). I did this with a range band in the line graphs and with a color difference in the maps (red for bellow and blue for above).

For stesp 1,2,4 I also opted to have a map on the bottom of the screen, with interaction effects for highlighting of country/region and year


# Feedback




# Resources
I based this visualiation on the EDA data and project developed for the Udacity Nanodegree. They are indcluded in this repository for conveniency:
* [R_Project.html](Source%20Data/R\_Project.html): This project builds on the EDA with R project under the same Nanodegree. This html reflects my exploratory data analysis and visualizations done in that project
* [Prep_data.html](Source%20Data/Prep\_data.html): This file documents the steps combining, preparing and cleaning the dataset before the R project analysis.
* _Source data/Original Data_  Folder: Here I include all original data as it was before any manipulation

The original data comes from data downloaded from the HDR report (for more details see: http://hdr.undp.org/en/data) and Regional and Development Classifications from UNSD (for details see: https://unstats.un.org/unsd/methodology/m49/overview/)
