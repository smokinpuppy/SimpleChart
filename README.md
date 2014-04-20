SimpleChart
========

Small jQuery Plugin to display a Chart of Plotted Data


Usage:
======

Include in Head Tag:

&lt;script type="text/javascript" src="http://code.jquery.com/jquery-latest.min.js"&gt; &lt;/script&gt;

&lt;script type="text/javascript" src="http://code.jquery.com/ui/1.10.4/jquery-ui.min.js"&gt; &lt;/script&gt;

&lt;script type="text/javascript" src="js/jquery.SimpleChart.js"&gt; &lt;/script&gt;


JavaScript / jQuery:

$('#demo1').SimpleChart({
	lineWidth: 2,				// Chart Line Width
	strokeColor: "#333",		// Axis Lines Color
	borderColor: "#333",		// Border Color
	borderWidth: 3,				// Border Width
	backgroundColor: "#FFF",	// Background color of chart
	backgroundImg: "css/jquery.SimpleChart/monthly_grid.png", // Background Image for chart (i.e Grid Layout)
	data: data,					// Default plot
	title: "Simple Chart",		// Default Title of chart
	titleFontSize: 16,			// Title Font size
	titleColor: "#FFF",			// Title Color
	showTitle: true,			// If True show title
	titleBGColor: '#006',		// Title Background Color
	xTitle: "",					// Title of X Axis
	yTitle: "",					// Title of Y Axis
	xTitleBGColor: '#006',		// Title X Axis background Color
	yTitleBGColor: '#006',		// Title Y Axis background Color
	xFontSize: 16,				// X Axis Title Font Size
	yFontSize: 16, 				// Y Axis Title Font Size
	xTitleColor: "#000",		// X Axis Title Color
	yTitleColor: "#000",		// Y Axis Title Color
	maxValX: 12,				// Maximum value of data XAxis
	maxValY: 100,				// Maximum value of data YAxis
	width: 500,					// Width of Graph
	height: 300,				// Height of Graph
	margin: 10,					// Margin between each graph
	showKey: true,				// Show chart key
	toolTip: ''					// If set, this will use jQuery Tooltip

});

Data(JavaScript):
var data = [
	{
		values:[						// Array of Plot Values
			{
				X:5,					// X Coordinate of Point 1
				Y:50					// Y Coordinate of Point 1
			},{
				X:10,					// X Coordinate of Point 2
				Y:100					// Y Coordinate of Point 2
			}							// And So on
		],
		color:"red",					// Color of the Line and Point
		title:"Red Color",				// Title of the line for the chart key
		action: "alert('Red Color');"	// Action if key is Clicked
	},{
		values:[
			{
				X:1,
				Y:60
			},{
				X:6,
				Y:70
			}
		],
		color:"blue",
		title:"Blue Color",
		action: "alert('Blue Color');"
	}
];


HTML:

&lt;div id="demo1" &gt;&lt;/div&gt; 
