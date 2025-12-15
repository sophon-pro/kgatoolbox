## Goal

Checks for `overlapping land parcels` across one or multiple layers, providing a fast and `efficient` alternative to topology-based validation.

## Summary

This tool is used to check the overlapping of land parcels. It can check one or more layers simultaneously. In addition to the usage of Topology, this tool facilitates the process of checking overlapped land parcels quickly and effectively. 

![parcel overlap check](../assets/parcel_overlap_check_ui.png)
## Illustration

![point to polygon](../assets/)

## Usage Note

* This tool can accept multiple land parcel layers input.
* Users can input one or more layers at the same time to check. 
* At the same time, there's option to show only the overlapped parcel feature which effectively aids the error inspecting process on that parcel.

## Parameters

This tool has some importances parameters as show in the table below.

| Parameter | Explanation | Data Type |
|:---------|:------------|:----------|
| Input_Feature | Input land parcel layers. | GPMultiValue |
| Highlight_Duplicated_Feature? (Optional) | Option to control how duplicated features are displayed.<br><br>• **Check:** Displays and labels only the duplicated parcels.<br>• **Uncheck:** Displays all parcels and selects duplicated parcels. | GPBoolean |
| Display_All_Features? (Optional) | Option to control parcel display behavior.<br><br>• **Check:** Redisplays all parcels and selects duplicated parcels.<br>• **Uncheck:** Maintains the current display. | GPBoolean |

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