## Project 3: Presidential Election Visualization
[![ScreenShot](http://roshanrshetty.github.io/Project3/Images/main.png)](http://roshanrshetty.github.io/Project1/Project1.mp4)

**Visualization Link:** http://roshanrshetty.github.io

### Data Description

We have used the follwing data fo this visualization
  1. Countywise election result for the years 2004,2008 and 2012.
  2. Countywise unemployment rate for the years 2004, 2008 and 2012.
  3. Countywise literacy rate for the years 2004, 2008 and 2012.
  4. 2016 election poll data.(Source: )
  

### Data Preprocessing

Data from multiple files had to be combined to get data for all 4 dimensions represented by the scatter plot. VLOOKUP was used to perform this.

### Features

#### 1. Different Tabs for Different Visualization

  We have implemented separate tabs for different visualizations, which not only helps the user to analyze but also reduces cognittive load.

#### 2. Slider

  The Slider enables the user to select visualization for different years. The slider implemented is a range slider, which enables the user to select between years.

![ScreenShot](http://roshanrshetty.github.io/Project3/Images/slider.PNG)

#### 3. Country Map

  we have used the country map for United States of America for our visualization. We have implemented both county-wise and state-wise visualization to present intricate details in an efficient manner.
  ![ScreenShot](http://roshanrshetty.github.io/Project3/Images/country.PNG)

#### 4. Zoomable Scatter Plot

  To display cluster information,we have also implemented a 2-axis zoomable scatterplot. This scatter plots displays a 4-dimensional data as described below:

   - The X-Axis represents unemployment rate.
   - The Y-Axis represents the win margin.
   - The Color of the circles indicate the winning party.
   - The Size of the circle represents the total number of voters in the county.
   
 The zooming features enables the user to view intricate details of the plots which are usually hidden in the over - all scatter plot.
  ![ScreenShot](http://roshanrshetty.github.io/Project3/Images/scatterplot.PNG)

#### 5. Time Series

  The Time Series enables the user to view changes in voting patterns over the years.
  ![ScreenShot](http://roshanrshetty.github.io/Project3/Images/timeseries.PNG)
  
#### 6. Animated Head to Head Bar
  The animated Head to Head Bar is a good way to visualize the battle for votes over time.
  ![ScreenShot](http://roshanrshetty.github.io/Project3/Images/header.PNG)
  
#### 7. Mini Map Selector

 The mini maps provides user with snapshots of the visualization over time. By double clicking on the mini map, the user can also load the vislauzation for the selected time.
 
 ![ScreenShot](http://roshanrshetty.github.io/Project3/Images/minimaps.PNG)
 
#### 8. Bubble Chart

  The Bubble Chart enables the user to view groupings in the data. These grouping help us understand the voting pattern. we can also use filters on these bubbles to view intricate details otherwise hidden by the visualization.
 ![ScreenShot](http://roshanrshetty.github.io/Project3/Images/split.PNG)


### Findings
![ScreenShot](http://roshanrshetty.github.io/Project3/Images/river.png)
![ScreenShot](http://roshanrshetty.github.io/Project3/Images/river.png)




### Work Distribution:

1. Naimisha Manikonda - Data Collection and Analysis For Effect of Unemployment Rate on Voting Patterns.
2. Andrew Salopek - Corelation between county votes to national results, predictive analysis.
3. Supra Jyotsna Jampa - Voter Transition between parties over the years.
4. Roshan Ramprasad Shetty - Election Poll Analysis.

Topics to be researched:
1. Gender based voting over the years.
2. Effects of population increase on election results ( new voters changed the results )


Work Accomplished:

1. Naimisha Manikonda - 
                - Found Datasets for Unemployment Rate and population
                - Link - http://www.fec.gov/pubrec/fe2014/federalelections2014.shtml  , http://www.presidency.ucsb.edu/showelection.php?year=2012 
                
2. Andrew Salopek<br>
                - working on county data for 2012 elections<br>
                - County Data across US 2012<br>
                - County Data across US 2008<br>
                - LINK TO HARVARD ELECTION DATA (CONCERNS ALL MEMBERS):  http://guides.library.harvard.edu/hks/campaigns_elections
              
                
3. Supra Jyotsna Jampa -
                - Found Data sets for previous elections, countywise data.
                - Researched over various visualization techniques suitable for the presentation.
                - Link: - http://elections.huffingtonpost.com/2012/results , https://www.theguardian.com/news/datablog/2012/nov/07/us-2012-election-county-results-download 
                
4. Roshan Ramprasad Shetty -
                - Collected dataset for 2016 polls. Link - https://www.kaggle.com/five-thirty-eight/2016-election-polls
                 



    
