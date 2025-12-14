## Goal



## Summary

This tool is used to standardize the attribute fields of land parcel layer to meet the requirement of MLMUPC. Those standard fields include ProDiCoVi (as text), UPRN (as short integer), parcel_no (as text), entry_dt (as date), update_dt (as date), history_dt (as date), status (as short integer), and digitizer (as text).

![point to polygon ui](../assets/parcel_cleaning.png)
## Illustration

![point to polygon](../assets/)

## Usage Note

* This tool has two process modes: i., cleaning data in place, ii., and cleaning and storing the data at a new location.
* It accepts multiple land parcel layer input.
* Fields that are not in the required fields can be dropped
* This tool also has an option to check and fill in the missing date value of any records in entry_dt field.
* If Clean and Copy? is checked, cleaned data will be stored at a new workspace (file geodatabase only).
* Before copying to new workspace, users can exclude owner field from the parcel data and be able to add suffix the name of output cleaned parcel. 

## Parameters

This tool has some importances parameters as show in the table below.

| Parameter | Explanation | Data Type |
|:---------|:------------|:----------|
| Clean_and_Copy? (Optional) | Specifies whether the cleaned data will be copied to a new output directory.<br><br>• **Check:** The cleaned data is copied from the current location to a new output directory.<br>• **Uncheck:** After cleaning, the data is not copied to a new output directory. | GPBoolean |
| Input_Feature_Class(es) | Input feature classes or layers to be cleaned. One or more feature classes are supported. | GPMultiValue |
| Digitizer's_Name (Optional) | Name of the land parcel digitizer. | GPString |
| Delete_Extra_Field(s) (Optional) | Specifies whether fields other than the required fields will be deleted.<br><br>• **Check:** All fields except allowable (required) fields are deleted.<br>• **Uncheck:** All original fields are retained. | GPBoolean |
| Check_Date_Field? (Optional) | Specifies whether the date field will be checked.<br><br>• **Check:** The **entry_dt** field is checked. Null values are updated with the latest date.<br>• **Uncheck:** The **entry_dt** field is not checked. | GPBoolean |
| Copy_Cleaned_Feature_Class_to_New_Workspace (Optional) | Specifies the output location for the newly copied, cleaned data. | DEWorkspace |
| Delete_Owner_Field (Optional) | Specifies whether the **Owner** field will be deleted.<br><br>• **Check:** The Owner field is removed from the copied data.<br>• **Uncheck:** The Owner field is retained. | GPBoolean |
| Change_Suffix? (Optional) | Specifies whether the suffix of the copied data name will be modified.<br><br>• **Check:** Enables the **Enter_Suffix** parameter to allow a custom suffix value.<br>• **Uncheck:** Uses the default suffix **(_Finished)**. | GPBoolean |
| Enter_Suffix (Optional) | Specifies the suffix to append to the copied feature class names. | GPString |

## Tool Demo

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

See toolbox [license package](pricing.md).

[Contact Sale :fontawesome-solid-paper-plane:](https://t.me/khmergrsacademy){ .md-button target="_blank" rel="noopener"}