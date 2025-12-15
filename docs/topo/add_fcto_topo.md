## Goal

Adding `Feature Classes` to an `existing Topology` and appy rules.

## Summary

This tool is used to add feature class(es) and Rule to existing Topology. 

There're three rules that were included.

* Rule 1: `Must Not Overlap (Area)`
* Rule 2: `Must Not Have Gap (Area)`
* Rule 3: `Must Not Overlap With (Area-Area)`

![point to polygon ui](../assets/add_fc_topo_ui.png)
## Illustration

![point to polygon](../assets/)

## Usage Note

* If the input topology already contains the input feature, tool won’t run.
* Chosen rules will be added to the input topology
* If feature classes share the boundary, their boundaries can be checked to find if they are overlapping with each other or not. 

## Parameters

This tool has some importances parameters as show in the table below.

| Parameter | Explanation | Data Type |
|:---------|:------------|:----------|
| Input_Topology | Existing topology to be checked. | DETopology |
| Check_Overlap_Boundary? (Optional) | Specifies whether the boundary of each polygon will be checked.<br><br>• **Check:** Input polygons are included in the boundary overlap checking process.<br>• **Uncheck:** Polygon boundaries are not checked. | GPBoolean |
| Input_Feature_Class(es) | Feature class(es) to be checked. | GPMultiValue |

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