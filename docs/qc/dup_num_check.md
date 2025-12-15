## Goal

Check the `duplicate number` in `UPRN field` of any `land parcel layer`.

## Summary

This tool is used to find duplicate value records in a selected numeric ID Field of land parcel feature class.

![point to polygon ui](../assets/parcel_dup_num_ui.png)
## Illustration

![point to polygon](../assets/)

## Usage Note

* The tool works with only integer field type where duplication finding can be proceeded.
* If duplicate value exists, those parcel features can be selected and highlighted.

## Parameters

This tool has some importances parameters as show in the table below.

| Parameter | Explanation | Data Type |
|:---------|:------------|:----------|
| Input_Feature_Class | One or more feature classes to be checked. | GPFeatureLayer |
| Choose_Field_to_check | Specifies the field to check for duplicate values. | Field |
| Select_Duplicated_Feature? (Optional) | Option to select and label duplicate features.<br><br>• **Check:** If duplicates are found, the features are selected and the UPRN value is labeled.<br>• **Uncheck:** Duplicate features are not selected; results are shown only in the tool message. | GPBoolean |
| Show_Label_for_only_Duplicated_UPRN? (Optional) | Option to label only duplicated UPRN values.<br><br>• **Check:** Only features with duplicated numbers are labeled.<br>• **Uncheck:** Labels remain unchanged and depend on other parameters. | GPBoolean |
| highlight_dup (Optional) | Option to highlight duplicate features for better visualization.<br><br>• **Check:** Duplicate features are highlighted.<br>• **Uncheck:** Duplicate features are not highlighted. | GPBoolean |

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

See toolbox [license package](../pricing.md).

[Contact Sale :fontawesome-solid-paper-plane:](https://t.me/khmergrsacademy){ .md-button target="_blank" rel="noopener"}