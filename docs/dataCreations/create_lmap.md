## Summary

The __Create or Export LMAP Layer__ generates a new LMAP-compliant feature class or exports an existing LMAP layer to a new file geodatabase. This tool is designed to standardize parcel capture workflows, enforce data quality rules, and streamline digitization activities within land management and mapping environments. This tool incorporates optional automation functions for unique identifiers, parcel numbering, and timestamp population. 

![create lmap](../assets/create_lmap.png)

Optional quality control logic helps maintain data integrity, including detecting duplicate UPRNs, automatically calculating parcel numbers, and inserting data entry timestamps.

## Illustration

Tool with parameters input

![create lmap layer](../assets/create_lmap_2.png)

Result after the creation (image below). Attribue Fields and theirs have been priorly set and data is ready to digitze. Data digitization and record value entry could be improved effectively with the the last three parameters. 

![create lmap layer](../assets/create_lmap_1.png)

## Usage Note

* If Export Feature? option is not checked, the tool creates an empty LMAP feature class with predefined schema and user-specified coordinate system.
* If Export Feature? is checked, the tool copies the selected LMAP layer to a new file geodatabase.
* The output feature class can be written in a file geodatabase (shapefile not recommended due to field name restrictions).
* The tool is typically used at the start of a digitization session or during controlled parcel update workflows.

## Parameters

This tool has three importances parameters as show in the table below.

| Parameter | Explanation | Data Type |
|:---------|:------------|:----------|
| Export_Feature? (Optional) | Dialog Reference<br>Determines whether to export existing LMAP feature classes to a new file geodatabase.<br><br>• **Unchecked:** The tool creates a new empty LMAP feature class.<br>• **Checked:** The tool exports the selected feature(s), ensuring schema consistency and applying optional automation rules.<br><br> | GPBoolean |
| Output_New_Feature (Optional) | Dialog Reference<br>The path and name of the new LMAP feature class to be created. Output as shapefile is not recommended. The output feature class name is restricted to follow the naming rule of LMAP – e.g. **V_01010101**, where the 8-digits number is the village code.<br><br> | DEFeatureClass |
| Output_Coordinate_System (Optional) | Dialog Reference<br>Specifies the coordinate system for the output feature class. PCS is recommended.<br><br> | GPCoordinateSystem |
| Digitizer's_Name (Optional) | Dialog Reference<br>Name of digitizer.<br><br> | GPString |
| Prevent_Duplicate_UPRN? (Optional) | Dialog Reference<br>Option to prevent duplicate UPRNs number.<br><br>• **Check:** Apply duplicate prevention to UPRN field.<br>• **Uncheck:** UPRN field can accept duplicate values.<br><br> | GPBoolean |
| Auto_Calculate_parcel_no (Optional) | Dialog Reference<br>Option to calculate **parcel_no** value automatically.<br><br>• **Check:** Automatically calculate parcel_no value during digitization session.<br>• **Uncheck:** parcel_no value will not be calculated automatically during digitization session.<br><br> | GPBoolean |
| Auto_Entry_Date (Optional) | Dialog Reference<br>Option to automatically enter the current date value to **entry_dt** field.<br><br>• **Check:** entry_dt value will be updated automatically.<br>• **Uncheck:** entry_dt value will not be populated.<br><br> | GPBoolean |
| Input_Features_to_Export (Optional) | Dialog Reference<br>Input LMAP feature to export.<br><br> | GPMultiValue |
| Output_Workspace (Optional) | Dialog Reference<br>Specify workspace location.<br><br> | GPComposite |


## Limitation

* Shapefile is not recommended.
* Output Feature class name is restricted to follow the naming rule of LMAP - eg: V_01010101, where the 8digits number is the village code.

## Demo

Learn how to use the tool

<iframe
  width="100%"
  height="600"
  src="https://www.youtube.com/embed/IgYOWnzz2lA"
  title="Land Parcel Data | Attribute Field Format Checking | KGA TOOLBOX"
  frameborder="0"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
  allowfullscreen>
</iframe>

## Purchase Toolbox

[Contact Sale :fontawesome-solid-paper-plane:](https:t.me/khmergrsacademy){ .md-button }