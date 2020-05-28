# TinyGPS
A compact Arduino NMEA (GPS) parsing library
For my application, I needed to know the value of the 6th comma, not just a true/false "Data Good"
I have forked this version and added the keyword fixedmode() that will return 0, 1, 2, etc... for the fix mode right before the satellite
count in a GGA string.
