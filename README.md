# Bigdata_Project
Part 1:  Design phase

Use the site below for the data that will be needed for this part of this project:
http://stat-computing.org/dataexpo/2009/the-data.html

Variable descriptions
	Name	Description
1	Year	1987-2008
2	Month	1-12
3	DayofMonth	1-31
4	DayOfWeek	1 (Monday) - 7 (Sunday)
5	DepTime	actual departure time (local, hhmm)
6	CRSDepTime	scheduled departure time (local, hhmm)
7	ArrTime	actual arrival time (local, hhmm)
8	CRSArrTime	scheduled arrival time (local, hhmm)
9	UniqueCarrier	unique carrier code

10	FlightNum	flight number
11	TailNum	plane tail number
12	ActualElapsedTime	in minutes
13	CRSElapsedTime	in minutes
14	AirTime	in minutes
15	ArrDelay	arrival delay, in minutes
16	DepDelay	departure delay, in minutes
17	Origin	origin IATA airport code

18	Dest	destination IATA airport code

19	Distance	in miles
20	TaxiIn	taxi in time, in minutes
21	TaxiOut	taxi out time in minutes
22	Cancelled	was the flight cancelled?
23	CancellationCode	reason for cancellation (A = carrier, B = weather, C = NAS, D = security)
24	Diverted	1 = yes, 0 = no
25	CarrierDelay	in minutes
26	WeatherDelay	in minutes
27	NASDelay	in minutes
28	SecurityDelay	in minutes
29	LateAircraftDelay	in minutes


Note that you have ancillary files on the site to convert the carrier and airport names.

http://stat-computing.org/dataexpo/2009/supplemental-data.html

 
Data Analysis Performed:

•	select a different year to extract the data from the site 

•	 load it  into Hadoop

•	determine the ten carriers with the highest delay time (in hours)

•	determine the ten carriers with the lowest delay time (in hours)


Capture the output results as follows:

Year	Carrier	Total Delay   	Arrival delay 	Departure Delay 	Carrier Delay	Weather
Delay	NAS Delay	Security Delay	Late Aircraft Delay

Phase 2: 

•	Select a representative sample of records  from each year

•	 Load it  into Hadoop as a Combine Years table

•	Add a new column called OnTime

•	Populate the OnTime column as follows
o	Put a “Y”   if the record has  a value of zero in the ArrDelay column
o	Put a “N”  if the record has  a non-zero value in the ArrDelay column

•	Select an analytics model that can predict which new records will be OnTime

•	Train, validate and test the analytics model with segments of your sample data

•	Prepare a presentation of the work done

