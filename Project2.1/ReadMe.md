#Projext 2: Text and Geo Spatial Visualization

## Data Preprocessing:

The data sets used for the visualization were from the 'WikiNews' and 'Huffington Post' websites.
The same approach was used for both the dataset for preprocessing.

Preprocessing in various phases as explained below:

1. **Getting Frequency Count For Every Word** : In this phase,
    - we read all the records avaiable in the datasets,
    - parse the extract words,
    - keep a counter for each word, that increments when the same word appears again.
    - Then we allow the user to download the same processed data as a .csv file using the 'FrequencyCounter - huffington.html' or 'FrequencyCounter.html' pages.
    
![ScreenShot](http://roshanrshetty.github.io/Project2.1/Images/preprocessing1.png)

2. **Getting All Record Numbers In Which A Word Appears** : In this phase,
    - we read all records in the dataset row by row,
    - for every word in the dataset, make seprate word entries with the record number.
    - if the same word is repeated in another row, we add the new record number to the already exisitng list.
    - then we allow the user to download the same processed data as a .csv file using the 'WordsInBlogs - huffington.html' and 'WordsInBlogs.html' pages.
   
![ScreenShot](http://roshanrshetty.github.io/Project2.1/Images/preprocessing2.png)    

3. **Indexing** : To make processing the faster, we have implemented an index for all the words. The Index has been implemented using elasticlunr.js. for searching relationships we make use of this index.
![ScreenShot](http://roshanrshetty.github.io/Project2.1/Images/index.png)

## Visualization:
The preproceesed data is presented in three ways:
### Wordle
A wordle(word cloud) is used to show all the main words asit is an effective way to visualize text with out any text overlapping.
#### Main Features of the Dynamic Wordle Implemented:
- Words grouped according to categories.
- Words size is directly proportional to the frequency of the words.   
- Hovering over a word highlights other words related to it in the Wordle.
- The slider can be used to get the wordle for the corresponding month.
- The wordle for a specified time range can be generated based on the range specified by the use.
![ScreenShot](http://roshanrshetty.github.io/Project2.1/Wordle.PNG)
### Time Series Visualization using Stacked Graph
- A stream graph is used as they indicate the relationships in the structure of data. They are used to represent the frequency of words over the period of time in this visualization.
- Stream graphs are uniue, such that data is appended on top of existing data, with the y-value of the area under the curve at x being the actual value of the data, so data with a larger area underneath the curve means more frequent, and data with a smaller area underneath the curve means less frequent.
- The graph uses many ticks that span the width of the visualization, in order to help the reader understand values in the chart.
- Implementation with various categories is shown below
![ScreenShot](http://roshanrshetty.github.io/Project2.1/Images/stacked graph.PNG)
![ScreenShot](http://roshanrshetty.github.io/Project2.1/Images/stacked graph.PNG)
![ScreenShot](http://roshanrshetty.github.io/Project2.1/Images/stacked graph.PNG)
### Force Directed Graph
A force directed graph is used to show the relationships between the nodes.
####Main Features of the Force Directed Graph Implemented:
- The relationships between words for the selected categories and time intervals are implemented.
![ScreenShot](http://roshanrshetty.github.io/Project2.1/Images/Force directed graph.PNG)
## Findings:
