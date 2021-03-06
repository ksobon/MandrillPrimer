#Line Chart

![](lineChart/lineChartImage.PNG)

##Data:

There are two ways of defining data for a Line Chart. First is to use a <b>CSV</b> file that was formatted in the following way: 

* First Column is always <b>Name</b> of the data point.
* Second Column is always the numerical <b>Value</b> for the data point.

###Example: 

![](areaChart/areaChartData.PNG)

Another possible way is to define the data in Dynamo directly and then use the node <b>LineChart.Data</b> to define all of the desired data points. Here's a potential sample of defining data in Dynamo:

![](lineChart/lineChartDataManual.PNG)

<blockquote>
Tip: As you can see in the image above, ALWAYS define number of Tick Marks in Chart Style to be <b>equal</b> or <b>less</b> than a number of data points. Specifying more ticks marks will result in an error. Default value is 10. 
</blockquote>

##Style:

Line Chart Style has a few simple things that can optionally be defined to control the visual appearance of the chart. First two inputs are for controling a color. You can either use a Dynamo Color node or a little bit of DesignScript syntax and a Code Block to define that input. Example: `DSCore.Color.ByARGB(1,220,180,20)`. <b>Width</b> and <b>Height</b> are integer inputs that by default are set to 1000px x 500px. The actual size of the chart is always a little smaller because of margins required for handling axis graphics etc. <b>TickMarksX</b> are an integer input. These define a number of data point names that are being displayed below X Axis. If you have a small data sample or really short names then it makes sense to render them all, but if you have a large data sample, to avoid overlapping text just enter a value that displays less names. Example of a Area Chart rendered above and its style: 

![](lineChart/lineChartStyle.PNG)
