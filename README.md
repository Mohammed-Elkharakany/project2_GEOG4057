# project2_GEOG4057

# Project Report on Elevation Data Extraction Script

## 1. Introduction

This project aims to extract elevation data from Google Earth Engine (GEE) for a set of points defined in a CSV file and store the results in a shapefile using ArcPy.

## 2. Code Development

### Modules Used
- **arcpy**: ArcGIS Python package for geospatial processing.
- **os**: Standard library for interacting with the operating system.
- **ee**: Google Earth Engine Python API for accessing GEE datasets and functionalities.
- **pandas**: Data manipulation and analysis library.

### Function Development
- **getGeeElevation**: This function extracts elevation data from GEE and saves it to a shapefile.
  - **Workspace**: Directory containing input and output files.
  - **CSV File**: Input CSV filename with point coordinates.
  - **Output Shapefile**: Name of the output shapefile.
  - **EPSG Code**: Spatial reference WKID code (default is 4326 for WGS GCS).

## 3. Usage Instructions

### Prerequisites
- ArcGIS with ArcPy installed.
- Google Earth Engine Python API.
- Pandas library.

### Running the Script
To run the script, use the following command:
```sh
python project2.py <workspace_directory> <csv_filename> <output_shapefile_name> <EPSG_code>

### Example: 
python project2.py E:\workspace\project2 boundary.csv pnt_elev2.shp 32119
