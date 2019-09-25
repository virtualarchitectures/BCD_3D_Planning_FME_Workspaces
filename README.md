# Building City Dashboards 3D Planning Tool - Workspace for Automating Data Preparation in FME

This repository includes FME workspaces for automating the preparation and processing of open data on planning information and Small Area Population Statistics in Dublin for use in the Building City Dashboards 3D Planning Tool.

## BCD 3D Model Layers
![BCD_3D_Planning_Open_Data_Layer_Workspace](images/BCD_3D_Planning_Open_Data_Layer_Workspace.PNG)

## Geolocate 3D Model
This workspace can be used to geolocate a 3D model that has been moved to the origin (0,0,0) or 'zeroed' for editing or visualisation in a 3D modelling or rendering software package. This can be used to correctly align 3D models and other spatial datasets that need to be accurately positioned relative to each other in a known geographic coordinate system.

Assumptions:
1. The 3D model is positioned close to the origin (0,0,0) in the the local coordinate space of a 3D modelling package. 
2. A file has been provided describing the spatial offset (x,y,z) that has been used to move the model from world coordinates to the local coordinate system of the 3D modelling package.
3. The world coordinate system is known.

![Geolocate3DModel](images/Geolocate3DModel.PNG)

## Set Model Origin By Geolocation 
This workspace can be used to set the position of a 3D model's pivot based on known geographic coordinates. This determines the point of the model from which rotation and scaling occurs when the model is imported into a 3D modelling package. This can be used to help align 3D models and other spatial datasets that need to be accurately positioned relative to each other in a known geographic coordinate system.

Assumptions:
1. The 3D model input contains geometry that is offset from the model origin (x,y).
2. That offset is described in coordinates derived from a recognised Coordinate Reference System (e.g. EPSG:2157 or other)
![SetModelOriginByGeolocation](images/SetModelOriginByGeolocation.PNG)

## Acknowledgements
On behalf of the Building City Dashboards project we gratefully acknowledge funding from **Science Foundation Ireland** under the Investigator’s Award Program. **Award number: 15/IA/3090**
