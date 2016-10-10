## Project 1: Time Series Visualization 


Please click to watch the overview video.

[![ScreenShot](http://roshanrshetty.github.io/Project1/Project1.PNG)](http://roshanrshetty.github.io/Project1/Project1.mp4)

**Visualization Link:** http://roshanrshetty.github.io

### Data Description

The data set used for visualization are:
 - State wise unemployment rates,
 - National unemployment rates.
 
The ***state wise unemployment rates*** dataset has been downloaded from https://piazza.com/class/issa77pf63o6oc?cid=12. The ***national unemployment rate*** dataset has been downloaded from http://data.bls.gov/timeseries/LNU04000000. The time range for both the above data sets is from 1st January 1976 to 31st July 2016 provided by the *Bureau of Labor Statistics*. A snapshot of the data is as follows:

[![ScreenShot](http://roshanrshetty.github.io/Project1/State wise unemployment rate.PNG)]

[![ScreenShot](http://roshanrshetty.github.io/Project1/National Unemployment rate.PNG)]



###Data Preprocessing###

The data avaialble had to be reformatted to be used for the visualization. The data was processed as follows:

***- Data Cleaning and Formatting***

1. The first step was to replace the month values represented as 'text' to it's corresponding numeric value. For example January was replaced with 1, May with 5 and so on.

2. The next step was to sort the dataset according to the ascending order of the year and months. This was done using the 'sort' functionality provided by Microsoft Excel.

***- Data Sepration***

1. The next steps was to seprate all the data for different states to different sheets in excel. This was done using 'Kutools' software.

2. Finally the seprate sheets were stored as different .csv files. I have used the following tutorial to do the same: https://www.youtube.com/watch?v=hnsL_01bHbU. The code for the macro is as follows:

  ```

    Sub Splitbook()
    MyPath = ThisWorkbook.Path
    For Each sht In ThisWorkbook.Sheets
    sht.Copy
    ActiveSheet.Cells.Copy
    ActiveSheet.Cells.PasteSpecial Paste:=xlPasteValues
    ActiveSheet.Cells.PasteSpecial Paste:=xlPasteFormats
    ActiveWorkbook.SaveAs _
    Filename:=MyPath & "\" & sht.Name & ".xls" & FileFormat:=xlCSV
    ActiveWorkbook.Close savechanges:=False
    Next sht
    End Sub

  ```

### Intresting Findings




