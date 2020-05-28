# TinyGPS
A compact Arduino NMEA (GPS) parsing library.

For my application, I needed to know the value of the 6th comma, not just a true/false "Data Good"
I have forked this version and added the keyword fixedmode() that will return 0, 1, 2, etc... for the fix mode right before the satellite
count in a GGA string.

  Fix quality: 0 = invalid
               1 = GPS fix (SPS)
               2 = DGPS fix
               3 = PPS fix
			       4 = Real Time Kinematic
			       5 = Float RTK
             6 = estimated (dead reckoning) (2.3 feature)
			       7 = Manual input mode
			       8 = Simulation mode
