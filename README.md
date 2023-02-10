# Landsat_clustering
Unsupervised classification of landuse in Landsat 8 (https://developers.google.com/earth-engine/datasets/catalog/LANDSAT_LC08_C02_T1_RT) in Google Earth Engine.

__Methodology__</br>
Landsat 8 contains 11 bands of wavelengths, which are scaled, calibrated at-sensor radiance. A composite cloudless image is first formed from the image set, which allows the study of larger area of interest. A clusterer using wekaKMeans (https://developers.google.com/earth-engine/apidocs/ee-clusterer-wekakmeans) was then trained and used over the area of study. 

Since it is unsupervised classification, further judgement by human is required to distinguish the content of each clusters. Comparisons over RGB image and NDVI layers were made, to determine the categories.

__Area of study__</br>
The area of study is near Abbortsford, BC, Canada.

__Google Earth Engine__</br>
The same code in the format of GEE Java can be cound in https://code.earthengine.google.com/bc184530bd533f950045acda243060d7?accept_repo=users%2Fujavalgandhi%2FEnd-to-End-Projects
