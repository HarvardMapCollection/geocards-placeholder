# Geocards Data

## Q & A

**What is the source of the spatial data?**

Administrative boundaries were sourced from the Geographical Atlas of the Russian Empire (GARE) published in the 1820s and adapted to reflect boundary changes made in the decades leading up to 1857. Town locations were also sourced from GARE. The points (towns) and polygons (provinces) are extraordinarily accurate representations of the data depicted on the atlas. GARE is recognized as the most comprehensive and accurate mapping of the empire prior to the middle of the 19th century. That said, the maps that compose the atlas were produced at different scales and in different projections. Together with the fact that the resolution of contemporary geospatial data is uniformly higher, this means that the despite the fact that this is the highest-quality data of its kind, users will find that the historical spatial data defines space slightly differently. Inaccuracy is not uniform across the data: it is more pronounced along the coastlines. (Additional note: The geojson and csv files for "towns" also include modern coordinate locations sourced from the Geonames gazetteer (geonames.org) with accompanying attestation URLs.)

**What is the projection of the spatial data?**

Data for this project is created in an [Equal Area Conic projection for Russia (8568)](https://spatialreference.org/ref/sr-org/albers-equal-area-russia/html/). The projection can be defined in a program like QGIS by [creating a custom coordinate reference system definition](https://gis.stackexchange.com/questions/20566/defining-new-custom-projections-in-qgis). 


**Why is the data provided in multiple formats?**

We provide the data in csv and geojson formats to make the data accessible to those who would like to work with it in GIS and non-GIS environments.

**What is the advantage of using the historical spatial data?**

Together, the geojsons (boundaries, towns, and rivers) offer a unique description of the historical space of the Russian Empire. Google Maps does not know where the boundaries of the empire were in 1857: but we do!


**Why are provinces and regions provided in separate geojsons?**

Each of the three regions is composed of multiple provinces. In the case of the Caucasus, the region contains territory that does not belong to any of the provinces (Chechnya/Dagestan). As a result, there is significant overlap in spatial coverage.

**Do the csv files contain the same data contained in the geospatial data, if the files have the same name?**

In some cases, yes, but not necessarily. Please consult the `file-notes.csv` for specifics.

**Do the geographic playing cards represent the entire space of the Russian Empire in the 1850s?**

Yes and no. There is a card for each province of the empire. There are also cards for the Russian America Company territories in Alaska (the Alaska Purchase would occur in 1867), the Kingdom of Poland, and the Grand Duchy of Finland. The card for the Caucasus region mentions the “territories of the mountaineers” (i.e., Chechnya/Dagestan) – territories that were not yet conquered or incorporated in an administrative sense (in contrast to the trans-Caucasian provinces for which there are cards. There is no card for the “Kirgiz” (Kazakh) steppe – an area which often shows up on maps of the empire at this time despite not yet being under Russian control.

**What if I do not understand a column heading?**

Check out `codebook.csv`.

**How do I cite the data?**

Use the automatically-generated citation from the [Imperiia Project Dataverse](https://dataverse.harvard.edu/dataverse/ImperiiaGIS)

**What if I have questions?**

Contact imperiia@fas.harvard.edu & @Imperiia