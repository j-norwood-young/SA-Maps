SA Maps
=======

South African Shapefiles, GIS data and other useful mapping stuff

CSIR Mesozones
--------------

![CSIR Mesozones](https://raw.github.com/j-norwood-young/SA-Maps/master/Examples/mesozones.png "CSIR Mesozones")

Source: http://www.gap.csir.co.za/download-maps-and-data

Provinces
---------

![Provinces](https://raw.github.com/j-norwood-young/SA-Maps/master/Examples/provinces.png "Provinces")

Source: http://www.demarcation.org.za/

Local Municipalities
--------------------

![Municipalities](https://raw.github.com/j-norwood-young/SA-Maps/master/Examples/municipalities.png "Municipalities")

Source: http://www.demarcation.org.za/

Districts
---------

![Districts](https://raw.github.com/j-norwood-young/SA-Maps/master/Examples/districts.png "Districts")

Source: http://www.demarcation.org.za/

Wards
-----

![Wards](https://raw.github.com/j-norwood-young/SA-Maps/master/Examples/wards.png "Wards")

Source: http://www.demarcation.org.za/

Schools
-------

![Schools](https://raw.github.com/j-norwood-young/SA-Maps/master/Examples/schools.png "South African schools with govt schools in red and private schools in white")

Source: http://www.education.gov.za/EMIS/EMISDownloads/tabid/466/Default.aspx

Command we used for making CSV smaller: 
```cut -d, -f 1,5-6,11,25-26,31,33,35,37,38,48-65,100-101 input.csv > output.csv```
Command we used for changing ``GIS_Lat`` and ``GIS_Long`` to latitude and longitude: 
```sed 's/GIS_Lat/latitude/' input.csv | sed 's/GIS_Long/longitude/' > output.csv```