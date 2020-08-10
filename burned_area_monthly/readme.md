### MODIS/Terra+Aqua Burned Area Monthly L3 Global 500 m Data Preparation

The Terra and Aqua combined MCD64A1 Version 6 Burned Area data product is a monthly, global gridded 500 meter (m) product containing per-pixel burned-area and quality information. The MCD64A1 burned-area mapping approach employs 500 m Moderate Resolution Imaging Spectroradiometer (MODIS) Surface Reflectance imagery coupled with 1 kilometer (km) MODIS active fire observations.

With these notebooks, you can create annual dataset from burned area monthly data.For this process we have 5 steps.

1. First notebook for [data download](https://github.com/orttak/Modis_Data_Preparation/blob/master/burned_area_monthly/Modis_Fire_Date_Download.ipynb) from website
2. Convert hdr file to [tif file](https://github.com/orttak/Modis_Data_Preparation/blob/master/burned_area_monthly/Modis_Fire_Date_Convert_to_TIF.ipynb)
3. Get the maximum value of each [tile](https://modis-land.gsfc.nasa.gov/MODLAND_grid.html) and create new [tif file](https://github.com/orttak/Modis_Data_Preparation/blob/master/burned_area_monthly/Modis_Fire_Date_Calculate_Mean.ipynb)
4. Create mosaic images which has sinusoidal projection and convert them to epsg:4326 with [this notebook](https://github.com/orttak/Modis_Data_Preparation/blob/master/burned_area_monthly/Modis_Fire_Date_Create_Mosaic.ipynb)
5. Create tiles from mosaic(epsg_4326) with [this notebook](https://github.com/orttak/Modis_Data_Preparation/blob/master/burned_area_monthly/Modis_Fire_Date_Create_Tiles.ipynb)
