Mean Soil Adjusted Vegetation Index 2 Calculation

The modified soil-adjusted vegetation index (MSAVI) and its later revision, MSAVI2, are soil adjusted vegetation indices that seek to address some of the limitation of NDVI when applied to areas with a high degree of exposed soil surface. The problem with the original soil-adjusted vegetation index (SAVI) is that it required specifying the soil-brightness correction factor (L) through trial-and-error based on the amount of vegetation in the study area. Not only did this lead to the majority of people just using the default L value of 0.5, but it also created a circular logic problem of needing to know what the vegetation amount/cover was before you could apply SAVI which was supposed to give you information on how much vegetation there was developed the MSAVI, and later the MSAVI2 to more reliably and simply calculate a soil brightness correction factor.

MSAVI2 = (2 * NIR + 1 – sqrt ((2 * NIR + 1)2 – 8 * (NIR - R))) / 2

Here we have used Sentinel-2 data. It is a wide-swath, high-resolution, multi-spectral imaging mission supporting Copernicus Land Monitoring studies, including the monitoring of vegetation, soil and water cover, as well as observation of inland waterways and coastal areas. Band 8 and Band 4 used and NIR and RED bands respectively along with QA60 band for cloud masking. Required MSAVI2 formula for Sentinel-2 will be:
MSAVI = (2 * Band 8 + 1 – sqrt ((2 * Band 8 + 1)2 – 8 * (Band 8 – Band 4))) / 2.

'geometry1' is the place 'Lakha' from Punjab. We can see the decrease in MSAVI 2 values from month of January to June. This could be possible because of wheat crop cultivation in initial months and harvesting in later. 'geometry2' is the place from Bihar where also we can se similar trends. 'geometry3' is Malkajgiri, Telangana area where we can observe different trend as compared to previous to regions. Here, MSAVI2 vsalues are kind of constant on linear curve fitting scale.
