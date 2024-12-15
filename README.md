# Geog 4057 Final Project Report
The coding part of the project was developed in Visual Studio (VS) Code, and primarily with meta, view, and column data. 
First, we expolored the json file and found that it consisted of a number of files, particulary sid, id, position, created_at, created_meta, updated_at, updated_meta, meta, the_geom, OBJECTID, ID, Cluster Letter, Shape.STArea(), and Shape.STLength(). We also were able to return a geometry object based on the Well-Known Text (WKT) string that was inputted and labelled it as poly1. Each row of data in the tax_json file was also visualized in VS Code. 
Data was written to a feature class. Our workspace link and name of the shapefile were established. The names of the three fields were understood (FID, Shape, ID). The field types were inputted into the code TEXT and LONG codes, but were outputted as the file names. id was changed to id_1 and ID was changed to id_10. Shape.STArea() was shortened to Shape_STAr, while Shape.STLength() was shortened to Shape_STLe. SHAPE@ was also added to the list of files by using the code "field_names.append('SHAPE@')". Inputting "field_names" into VS Code showed the final list of updated files, with their new names and the manually added files. 
Data was added to a feature class. InsertCursor was used in the code to establish a new feature class, while each value was processed, except the value that belongs to number 8 (it was skipped). "for row in tax_json['data']:
    print(row)" printed the metadata information for each value/file. 
    Moving over to ArcGIS Pro, notax2_fc.shp (shapefile) was added to the map. A new python toolbox was created, where the data of it was edited in VS Code. It was then refreshed and updated in ArcGIS Pro so the edits were seen in both programs. 




In the repository of the project, write a report including how the code was developed and how to use the code











