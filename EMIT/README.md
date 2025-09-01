# EMIT
Classfication code to run on Hyperspectral EMIT data

Download EMIT data from: https://search.earthdata.nasa.gov/search?q=emit

Download emit_tools module (needed to open the .nc file): https://github.com/nasa/EMIT-Data-Resources/tree/main/python/modules

Order of code files:
1. Convert the netcdf files to geotiff
2. Clip the files to the ROI (region of interest)
3. Mosaic the images to get one scene and filter out nan values and bands that cause noise
4. Perform the classification
5. Run the accuracy assessment 

Additional scripts:
4. Export the RGB to display true colour in ArcGIS Pro (optional)

Packages needed: 

conda install -c conda-forge earthpy

conda install -c conda-forge folium

conda install -c conda-forge fiona

conda install -c conda-forge gdal

conda install -c conda-forge geopandas

conda install -c conda-forge pandas

conda install -c conda-forge numpy

conda install -c conda-forge rioxarray

conda install -c conda-forge rasterio

conda install -c conda-forge scikit-learn

conda install -c conda-forge tqdm


# Alternative
pip install earthpy

pip install folium

pip install fiona

pip install gdal

pip install geopandas

pip install pandas

pip install numpy

pip install rioxarray

pip install rasterio

pip install scikit-learn

pip install tqdm

