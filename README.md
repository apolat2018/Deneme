
<p align="center">
  <b>ANNEX</b>
</p>
<p><strong>User Interfaces and Processes of Landslide Susceptibility Tool Scripts</strong></p>
<p>Figures</p>

Fig. 1 User interface of Data Preparation script
Fig. 2 User interface of FR script
Fig. 3 User interface of IV Script
Fig. 4 User interface of Create LSM and Calculate ROC script.
Fig. 5 User interface of LR script.
Fig. 6 User interface of tuning LR script
Fig. 7 User interface of RF script.
Fig.  8 User interface of Tuning RF script.
Fig.  9 User interface of MLP script.
Fig. 10 User interface of tuning MLP script.
*Tables
Table 1 Description of input parameter and processes of Data Preparation Script. 
Table 2 Description of input parameter and processes of FR Script.
Table 3 Description of input parameter and processes of IV Script.
Table 4 Description of input parameter and processes of Create LSM and Calculate ROC script.
Table 5 Description of input parameter and processes of LR script.
Table 6 Description of input parameter and processes of tuning LR script.
Table 7 Description of input parameter and processes of RF script.
Table 8 Description of input parameter and processes of Tuning RF script.
Table 9 Description of input parameter and processes of MLP script.
Table 10 Processes of tuning MLP script.

<p align="center">
  <img width="793" height="691" src="https://github.com/apolat2018/Deneme/blob/master/fig1.png">
</p>
<p align="center">
  Figure 1. User interface of Data Preparation script
</p>

**DESCRIPTION OF INPUT PARAMETERS**
|Parameter|Explanation|Data Type|
|:-------- |:----------- |:----------|
|The_Folder_of_the_parameters|The name of the parameter, raster files must begin with "rec" rec_aspect, rec_slope etc.|Folder|
|Landslide_file__shp_	|Landslides file(.shp) must be polygon type|Shapefile|
|Area_file__shp_	|Desired area file (.shp)	|Shapefile|
|cell_size|	Cell size of the output raster data.|	Cell Size|
|Data_Type|	Two type of data is enabled for use in susceptibility analysis. These values are class values and normalized frequency ratio. 	|String|
|Train_Validation_Split_size|	Split size of data as train and validation. Percentage of input landslide data|	Double|

**THE PROCESSES OF DATA PREPARATION SCRIPT**
|:---------|
|[u'rec_asp', u'rec_crv', u'rec_eleva', u'rec_lito', u'rec_ls', u'rec_ndvi', u'rec_ridge', u'rec_slp', u'rec_tri', u'rec_twi']|
|10 raster data imported as parameter|
|Area is converting to Raster|
|Raster is converting to Point|

**PREPARING TRAIN DATA AND VALIDATION DATA**
|:---|
|Clipping landslides|
|landslide pixels are converting to point|
|Extracting landslide pixels|
|clp_asp is processing|
|Creating raster files with Normalized Frequency Ratios and Normalized Information Values|
|clp_asp is finished|
|Preparing Data for Frequency ratio value|
|Saving TRAINING data as train_fr.csv|
|Preparing Data for information value|
|Saving TRAINING data as train_iv.csv|
|Extracting Values to Point|
|Extracting finished|
|Saving ALL data as pre_iv.csv|
|Validation landslide is saving as test_1.shp|
|Completed script prepare...|
|**Elapsed Time: 14 minutes 15 seconds**|
