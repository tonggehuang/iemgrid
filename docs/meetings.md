30 Nov 2016
-----------
 - Two additional Dell racks were present to help with the data processing
   requirements.
 - They are using processing.js on their end to do some of the work
 - They are storing data utilizing RGB to store three variables within one
   file.
 - They demonstrated a Tableau around Omaha showing fancy graphics
 - They had a display showing data around crashes within the database
 - There is bluetooth sensors now on the DOT blades, so blade position data
   should be good now.
 - The plow imagery provides a great dataset for looking into crashes
 - Discussion about sources of precip type forecasts and the national blend of
   models does not appear to address this, yet.
 - [x] no units denoted on github README?  gasp, accurate, but I thought I
   wrote more details on this :(

04 Feb 2016
-----------
 - A new format was proferred with it being JSON, we worked through an example
 - They want individual forecast hours in a single file
 - They suggested having the archive data in CSV and current, future in JSON
 - An issue of having excessive zeros in the file was mentioned, I am unsure of
   it and asked to see an example
 - Some Aurora projects were discussed, but they were outside of my area.

 07 Jan 2016
----------- 
 - Mike Fowle (DMX SOO) showed a decision support tool for winter wx
   http://weather.gov/wrh/tavel/?wfo=sds
 - It was noted that currently $400b in freight crosses Iowa each year
 - An email list will be established to support this group's work
 - Primary focus is initial investigations on Interstates
 - DOT has an advisory speed project whereby signs will note to slow down
 - Fowle noted that lots of accidents in SD happen in Nov due to deer
 - daryl is the slow cog
 - Arujn has some image processing stuff with deep learning
 
12 Nov 2015
-----------
- Discussion of the data format and other aux issues
- [ ] Additional variables
  - Gridded NWS Watch Warning Advisory codes
- xml file wrapped with <wx>
- time expressed as ISO
- Discussion of timing of forecasts
- use English units in xml

29 Oct 2015
-----------
- This was the initial meeting to get work kicked off
- NTRANS is interested in anything that impeeds traffic flow
- For realtime purposes, there is some latencies involved with their other
vendors of data.  They need time to collect up enough samples to make for
appropriate statistics.
- They are looking for an XML feed of data
- They use UTMz15, but are likely OK with Lat/Long WGS84
- Decision was to go with 1 Jan 1997 as start date
- 5 minute interval in time
- Timestamps would be presented as UTC
- Express Precipitation in Hourly Rates
- [ ] Variables to deliver
  - Precip type (int flag)
  - 2m Air Temperature
  - 2m Dew Point
  - 10m Wind Speed
  - 10m Wind Direction (no u/v components)
- [ ] Additional Variables that will have lots of caveats
  - Visibility, understanding that I can't go down below 1/8 mile
  - Pavement Temp, very crude regridding of RWIS data
  - Solar Radiation (2014 onward)
  - Snow Depth would be once per day
- MADIS was discussed, but no real conclusion reached about it
- [ ] deliver format example by 20 November
- [ ] stand-up IEM TMS services for these variables
- usage of NDFD grids to drive forecast grids of the above
