# Links to the Tableau Public workbooks
Version 1: 
https://public.tableau.com/views/HDR_v1/HDIStory?:embed=y&:display_count=yes&publish=yes



# Summary
This visualization shows the progress of the Human Development Index over time. The focus is on the fact that while World average has increased, and most countries increased their own HDI, the gap (i.e. difference) between regions remains. In particular, Africa is constantly at the bottom and Europe constantly at the top for the HDI and its 3 components.


# Design
## Version 1:
I opted to have the Tableau Story told in 4 steps: 
* Step 1: World averages
* Step 2: Break down by Region
* Step 3: Evolution, by Region, of the 3 components
* Step 4: Break down by Country, within region

Since all steps involve evolution over time, I opted to show these with line graphs, wtih averages per year. There is one line for World Average, one line for each Region or one line for each Country, depending on the Step.

For all visualizations I opted to highlight the limit point above which it is considered (at least) medium human development (0.550). I did this with a range band in the line graphs and with a color difference in the maps (red for bellow and blue for above).

For steps 1,2,4 I also opted to have a map on the bottom of the screen, with interaction effects for highlighting of country/region and year. The map is informative as can show how regions evolve and help find a specific country of interest, in particular in the last step where there are many lines.

For Step 4, I opted to have the countries grouped by region to improve readability.

# Feedback
I requested feedback from a work colleague. This is what he wrote, after interacting with the first version:

*What do you notice in the visualization?*
*	Slow loading, and slow clicking frequently (like reset) *An unexpected error occurred. If you continue to receive this error please contact your Tableau Server Administrator. Session ID: 202E441743324710B747D2F57E7CAC37-0:1 Uncaught TypeError: Cannot read property 'zoneId' of null*
*	Years in the top bar can be click on, presumably to change data year, but don’t work or change map view only VERY slowly. Can only change year on top right which wasn’t obvious at first. 
*	It starts in 1996, convention would be to start in most recent year?
*	Map seems much to small relative to the page, making it tricky to hover on without zooming, which is slightly annoying
*	Zooming ‘crops’ the map, I prefer to see the whole map, so enlarging the area of maps space would be ideal
*	HDI is used, grading countries with colors, low red high blue. This is easy and clear to me. Personally I would use traffic light red green 
*	I don’t see the point of ‘keep only’ option when I click a country
*	I wish I could ‘play’ the data (like gapminder) to view HDI changes over time by whole world, or by region, or by a selector of countries
*	You have given regions colors (top right) but these should not have colors – it confuses the color interpretation of your HDI gradient. 

*What questions do you have about the data?*

*What relationships do you notice?*

*	I can see HDI increases over time, but basically patterns remain. While developing got more developed (especially asia), these countries still have lower HDI than, say Europe, which is to be expected. 

*What do you think is the main takeaway from this visualization?*
*	HDI of most countries has improved in 20 years in all regions. 

* *Is there something you don’t understand in the graphic?*
 * No 




# Resources
I based this visualiation on the EDA data and project developed for the Udacity Nanodegree. They are indcluded in this repository for conveniency:
* [R_Project.html](Source%20Data/R\_Project.html): This project builds on the EDA with R project under the same Nanodegree. This html reflects my exploratory data analysis and visualizations done in that project
* [Prep_data.html](Source%20Data/Prep\_data.html): This file documents the steps combining, preparing and cleaning the dataset before the R project analysis.
* _Source data/Original Data_  Folder: Here I include all original data as it was before any manipulation

The original data comes from data downloaded from the HDR report (for more details see: http://hdr.undp.org/en/data) and Regional and Development Classifications from UNSD (for details see: https://unstats.un.org/unsd/methodology/m49/overview/)

I also consulted and downloaded this viz to get inspiration for some functionality:
https://public.tableau.com/profile/susan.li#!/vizhome/HappyPlanetIndex_2/2016WorldHappinessStory

