# Less popular activities with similar neighbors
 
A client  want to create a business with high potential in a European city among Paris, London and Madrid.
He wants to identify cities that are similar and identify the neighborhoods that are most similar and identify activities that, although having expanded elsewhere are still slow to grow in other similar areas.
He believes it is an interesting niche with analyzer.
He therefore suggests that we carry out this study and present the main activities which do not all evolve at the same speed in the 5 largest similar districts of Paris, London and Madrid.


1. Data collection:

A- extraction of districts without coordinates (Latitude and logitude)
We have extracted the districts without coordinates of the different cities individually in the websites below:

Given the reduced size of the different data sources, we opted for the manual copy / paste method in order to save time, unlike the other methods (BeautifullSoup ...) which are advantageous in the case of a very large number of data.
The extracted data will be gathered in a single CVS file.

- Extraction of Madrid neighborhoods from the site:
https://fr.db-city.com/Espagne--Madrid--Madrid--1

- Extraction of paris districts:
https://fr.wikipedia.org/wiki/Liste_des_quartiers_administratifs_de_Paris

- Extraction of the districts of London:
- https://en.wikipedia.org/wiki/List_of_areas_of_London



B- Update of our district file with GPS coordinates.

Two methods seemed more affordable to us for collecting location data.
- The method with the Geocoding API: https://developers.google.com/maps/documentation/geocoding/start
- The method with the tools https://geocode.localfocus.nl/

To save time (although we practice with the geocoding method), we have used the https://geocode.localfocus.nl/ tool where we have uploaded our previously extradited data.

After some restatements, we have obtained, the cities, the districts and the GPS coordinates of the different cities (Paris, Madrid and London) attached

https://s3.amazonaws.com/csvpastebin/uploads/b219de95b1e1a73911b6443d5fd85cc1/Data_final.csv

The first phase of processing and visualization of the districts in question is presented in our notebook below:
