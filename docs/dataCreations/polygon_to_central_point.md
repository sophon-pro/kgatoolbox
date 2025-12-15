## Goal

Create ```central point``` feature class from ```input polygon```.

## Summary

This tool converts ```polygon features``` into representative ```central points```. For each polygon, the tool determines a centroid and creates a corresponding point in the output feature class. There’s an option to retain all attributes or keep only the polygon ID and can optionally calculate __X/Y__ or __Lat/Lon__ fields based on the input Coordinate System. 

The tool can also generate a separate coordinate table as well.

![point to polygon ui](../assets/polygon_centpoint_ui.png)
## Illustration

![point to polygon](../assets/polygon_centpoint.png)

## Usage Note

* Input must be a ```polygon feature class```.
* The output is a ```central point feature class``` of each polygon.
* If “Drop unrelated fields except ID Field?” is enabled, another parameter called ```Choose ID Field``` appear which let user pick an ID field and all fields inherited from input polygon will be removed.
* If the coordinate calculation option is enabled, ```X/Y or Latitude/Longitude fields``` will be added depending on the coordinate system.
* __“Export Coordinate as Table?”__ creates an additional table listing polygon identifiers and their calculated coordinates.

## Parameters

This tool has some importances parameters as show in the table below.

| Parameter | Explanation | Data Type |
|:---------|:------------|:----------|
| Input_Feature | The polygon dataset from which central (centroid) points will be generated. | GPFeatureLayer |
| Drop_unrelated_fields_except_ID_Field? (Optional) | Option to remove all fields in the output point feature that are inherited from the input feature.<br><br>• **Checked:** Drops all fields and enables the **Choose_ID_Field** parameter.<br>• **Unchecked:** Keeps all fields. | GPBoolean |
| Choose_ID_Field (Optional) | Option to choose the ID field to keep when **Drop_unrelated_fields_except_ID_Field?** is enabled. | Field |
| Output_Point_Feature_Class | The location and name of the point feature class that will be created. | DEFeatureClass |
| Calculate_XY_or_LatLon (Optional) | Adds coordinate fields to the output feature class (X/Y for projected data or Lat/Lon for geographic data).<br><br>• **Check:** Coordinates are calculated automatically based on the output CRS (PCS → X/Y, GCS → Lat/Lon).<br>• **Uncheck:** No coordinate fields are calculated. | GPBoolean |
| Export_Coordinate_as_Table? (Optional) | Option to create a standalone table containing polygon IDs and their corresponding centroid coordinates.<br><br>• **Check:** Creates a standalone table.<br>• **Uncheck:** No table is exported. | GPBoolean |
| Specify_Table_output_Location (Optional) | The location and name of the table that will be created. | DETable |

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