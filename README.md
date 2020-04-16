# Deneme
Bu bir denemedir. 
<head>
<title>Page Title</title>
</head>
Bu şekilde şekil eklenebiliyor

<p align="center">
  <img width="512" height="327" src="https://github.com/apolat2018/Deneme/blob/master/deneme.JPG">
</p>

figure 1 eklendi:

<p align="center">
  <img width="535" height="273" src="https://github.com/apolat2018/Deneme/blob/master/fig1.jpg">
</p>

|DESCRIPTION OF INPUT PARAMETER|
|-------------------------------|
|Parameter|	Explanation|	Data Type|
|:---||:---||:---|
|The_Folder_of_the_parameters|The name of the parameter, raster files must begin with "rec" rec_aspect, rec_slope etc.|Folder|
|Landslide_file__shp_	|Landslides file(.shp) must be polygon type|Shapefile|
Area_file__shp_	Desired area file (.shp)	Shapefile
cell_size	Cell size of the output raster data.	Cell Size
Data_Type	Two type of data is enabled for use in susceptibility analysis. These values are class values and normalized frequency ratio. 	String
Train_Validation_Split_size	Split size of data as train and validation. Percentage of input landslide data	Double
THE PROCESSES OF DATA PREPARATION SCRIPT
[u'rec_asp', u'rec_crv', u'rec_eleva', u'rec_lito', u'rec_ls', u'rec_ndvi', u'rec_ridge', u'rec_slp', u'rec_tri', u'rec_twi']
10 raster data imported as parameter
Area is converting to Raster
Raster is converting to Point
PREPARING TRAIN DATA AND VALIDATION DATA
Clipping landslides
landslide pixels are converting to point
Extracting landslide pixels
clp_asp is processing
…………………..
Creating raster files with Normalized Frequency Ratios and Normalized Information Values
clp_asp is finished
…………………..
Preparing Data for Frequency ratio value
Saving TRAINING data as train_fr.csv
Preparing Data for information value
Saving TRAINING data as train_iv.csv
Extracting Values to Point
Extracting finished
Saving ALL data as pre_iv.csv
Validation landslide is saving as test_1.shp
Completed script prepare...
Elapsed Time: 14 minutes 15 seconds
