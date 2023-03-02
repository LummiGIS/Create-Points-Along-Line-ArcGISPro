# Create-Points-Along-Line-ArcGISPro
A geoprocessing tool to create points along a feature class at user defined intervals.

ArcGIS Pro v3 Sripting toolbox tool.
This geoprocessing tool takes a line feature class in a Cartesian coordinate reference system (CRS) and creates a new feature class of points at user defined intervals. The points are distributed along the input lines at equal interval distances. Starting with the first node of a line record, a point is created at the start node position with a distance value of 0. Using the user-defined interval distance, a point is added at each graduation along the line. Each point is attributed with the total cumulative distance from the start node. Points are only created at interval distances so if a line segment is greater than the interval distance that portion of the line is not given a point. After completing the first record, the above process is repeated for the next record.


This tool does not work with multi-part geometries, or geographically projected data. It was tested using WaSPN and UTM 10N projections.
The division values are based on the lines CRS units of measure and not the CRS of the data frame.


This tool in an ArcGIS Pro implementation of the ArcGIS Desktop tool available here:   https://github.com/LummiGIS/Create_Points_Along_A_Line_Feature_Class


https://github.com/LummiGIS/Create-Points-Along-Line-ArcGISPro/blob/main/img/divideline.png|alt=octocat

