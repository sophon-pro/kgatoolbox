## Goal

Count the ```total features``` within the input ```feature classes```.

## Summary

This tool `counts features` in multiple `feature classes` and optionally exports the results to a CSV file.

![point to polygon ui](../assets/count_feature_ui.png)
## Illustration

![point to polygon](../assets/count_feature.png)

## Usage Note

* Inputs: Provide a list of feature classes. Enable CSV export and specify the file path if needed.
* Execution: The tool counts features for each class, displays details in messages, and calculates the total.
* Output: Feature counts and the total are displayed. And optionally, results can be saved as a CSV file with Feature Class and Count columns.

## Parameters

This tool has some importances parameters as show in the table below.

| Parameter | Explanation | Data Type |
|:---------|:------------|:----------|
| Input_Feature_Class(es)_to_count | One or more feature classes to be counted. | GPMultiValue |
| WriteCSV (Optional) | If checked, each counted result will be written to a CSV file. | GPBoolean |
| OutputCSV (Optional) | Specifies the output directory and file in supported formats (**.csv**, **.txt**). | GPComposite |

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