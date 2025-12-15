## Goal

Check the `overall state` of parcel number in a land parcel layer.

## Summary

This tool is used to check the land parcel number information. The information to check includes total parcel feature, start and end parcen number, total duplicate number, and total missing number. Parcel number information can be exported as report in text file.

![point to polygon ui](../assets/parcel_num_anal_ui.png)
## Illustration

![point to polygon](../assets/)

## Usage Note

* This tool may not work for fields that have field type of Text or another field except numeric field.

## Parameters

This tool has some importances parameters as show in the table below.

| Parameter | Explanation | Data Type |
|:---------|:------------|:----------|
| Input_Feature_Class | Input feature class or table to be checked. | GPMultiValue |
| Check_Field_to_Check | Choose the field containing parcel numbers to check. | Field |
| Generate_Report? (Optional) | Option to export the result as a report.<br><br>• **Check:** Exports the report to a text file.<br>• **Uncheck:** No report is exported. | GPBoolean |
| Output_Report (Optional) | Specifies the location and name of the output report file. | DETextFile |

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