#Bar Chart

![](barChart/barChartImage.PNG)

##Data:

There are two ways of defining data for a Bar Chart. First is to use a <b>CSV</b> file that was formatted in the following way: 

* First Column is always <b>Name</b> of the data point.
* Second Column is always the numerical <b>Value</b> for the data point.

###Example: 

![](barChart/dataSample.PNG)

Another possible way is to define the data in Dynamo directly and then use the node <b>BarChart.Data</b> to define all of the desired data points. Here's a potential sample of defining data in Dynamo:

![](barChart/manualData.PNG)

<blockquote>
Tip: As you can see in the image above, ALWAYS define number of Tick Marks in Chart Style to be <b>equal</b> or <b>less</b> than a number of data points. Specifying more ticks marks will result in an error. Default value is 13. 
</blockquote>

##Style:

##Other:
