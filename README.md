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

School data includes all the schools in South Africa according to the Dept of Education (data for 2012 and 2013), plus education districts. Please note that education districts don't seem to be 100% accurate, especially in North West, and there are no school district names provided by the Department of Basic Education for Mpumalanga. Weird.

![Schools](https://raw.github.com/j-norwood-young/SA-Maps/master/Examples/schools.png "South African schools with govt schools in red and private schools in green")

Source: http://www.education.gov.za/EMIS/EMISDownloads/tabid/466/Default.aspx

Command we used for making CSV smaller (2012 data): 
```cut -d, -f 1,5-6,11,25-26,31,33,35,37,39,48-65,100-101 input.csv > output.csv```

Command we used for making CSV smaller (2013 data): 
```cut -d, -f 1,4-5,10,13,15,29-30,40,42,44,45-46,50,58-75,116-118 National_Schools_Q1_2013.original.csv > National_Schools_Q1_2013.csv```

Command we used for changing ``GIS_Lat`` and ``GIS_Long`` to ``latitude`` and ``longitude`` (2012 data only): 
```sed 's/GIS_Lat/latitude/' input.csv | sed 's/GIS_Long/longitude/' > output.csv```

Subplaces
---------

Like, suburbs, dude! 

Please note that these are ZIPPED UP becaue of Git's 100MB file limit! If you make changes, zip it up again and add the zip, not the subplace folder. 

Source: Statistics SA Census 2011 Spatial Metadata

![Subplaces](https://raw.github.com/j-norwood-young/SA-Maps/master/Examples/subplaces.png "Subplaces")

Main Places
-----------

Please note that these are ZIPPED UP becaue of Git's 100MB file limit! If you make changes, zip it up again and add the zip, not the main place folder. 

Source: Statistics SA Census 2011 Spatial Metadata

![Main places](https://raw.github.com/j-norwood-young/SA-Maps/master/Examples/mainplaces.png "Main places")
