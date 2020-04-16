
<p align="center">
  <b>ANNEX</b>
</p>
<p><strong>User Interfaces and Processes of Landslide Susceptibility Tool Scripts</strong></p>
<p>Figures</p>

- Fig. 1 User interface of Data Preparation script
- Fig. 2 User interface of FR script
- Fig. 3 User interface of IV Script
- Fig. 4 User interface of Create LSM and Calculate ROC script.
- Fig. 5 User interface of LR script.
- Fig. 6 User interface of tuning LR script
- Fig. 7 User interface of RF script.
- Fig.  8 User interface of Tuning RF script.
- Fig.  9 User interface of MLP script.
- Fig. 10 User interface of tuning MLP script.

<p>Tables</p>

- Table 1 Description of input parameter and processes of Data Preparation Script. 
- Table 2 Description of input parameter and processes of FR Script.
- Table 3 Description of input parameter and processes of IV Script.
- Table 4 Description of input parameter and processes of Create LSM and Calculate ROC script.
- Table 5 Description of input parameter and processes of LR script.
- Table 6 Description of input parameter and processes of tuning LR script.
- Table 7 Description of input parameter and processes of RF script.
- Table 8 Description of input parameter and processes of Tuning RF script.
- Table 9 Description of input parameter and processes of MLP script.
- Table 10 Processes of tuning MLP script.

<p align="center">
  <img width="793" height="691" src="https://github.com/apolat2018/Deneme/blob/master/fig1.png">
</p>
<p align="center">
  <b>Figure 1.</b> User interface of Data Preparation script
</p>
<p align="center">
  <b>Table 1.</b> Description of input parameter and processes of Data Preparation Script. 
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
|*Elapsed Time: 14 minutes 15 seconds*|

<p align="center">
  <img width="793" height="691" src="https://github.com/apolat2018/Deneme/blob/master/fig2.png">
</p>
<p align="center">
  <b>Figure 2.</b> User interface of FR script
</p>

<p align="center">
  <b>Table 2.</b> Description of input parameter and processes of FR Script. 
</p>

**DESCRIPTION OF INPUT PARAMETER**

|Parameter|	Explanation|	Data Type|
|:---|:---|:---|
|Rec_folder|	Select the folder where the Parameter files (Reclassed raster data) are located.| 	Folder|
|Save_Folder|	Susceptibility map and ROC graph is saving this Folder|	Folder|
|Coordinate_system|	Coordinate System of output raster|	Coordinate System|
|cell_size|	Cell size of the raster|	Cell Size|
**THE PROCESSES OF FREQUENCY RATIO SCRIPT**
|Starting Frequency Ratio Analysis...|
|Analysis finished|
|Susceptibility Map was created in Save folder as FR_sus raster file|
|ROC calculation is starting.....|
|Success rate is: 72.7066604308|
|prediction rate is: 70.9536573075|
|AUC Graph is saved as auc_fr.png|
|Completed script FRanalysis...|
*(Elapsed Time: 26,56 seconds)*

<p align="center">
  <img width="793" height="691" src="https://github.com/apolat2018/Deneme/blob/master/fig3.png">
</p>
<p align="center">
  <b>Figure 3.</b> User interface of IV script
</p>

<p align="center">
  <b>Table 3.</b> Description of input parameter and processes of IV Script. 
</p>

**DESCRIPTION OF INPUT PARAMETER**

|Parameter|	Explanation|	Data Type|
|:---|:---|:---|
|Rec_folder|	Select the folder where the Parameter files (Reclassed raster data) are located.| 	Folder|
|Save_Folder|	Susceptibility map and ROC graph is saving this Folder|	Folder|
|Coordinate_system|	Coordinate System of output raster|	Coordinate System|
|cell_size|	Cell size of the raster|	Cell Size|
**THE PROCESSES OF FREQUENCY RATIO SCRIPT**
|Starting Information Value Analysis...|
|Analysis finished|
|Susceptibility Map was created in Save folder as IV_sus raster file|
|ROC calculation is starting.....|
|Success rate is: 72.942322706|
|prediction rate is: 71.8463442428|
|AUC Graph is saved as auc_IV.png|
|Completed script IVanalysis...|
*(Elapsed Time: 15,67 seconds)*
