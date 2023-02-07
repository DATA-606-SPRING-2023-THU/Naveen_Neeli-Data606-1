## About the project

## Goal
My initial thoughts about the project is to predict taxi fares which would be helpful for the user to plan his/her trip. <br>

## Model
I would like to apply couple of machine learning algorithms like Linear regression, XBoost, RandomForest on the data and compare their performances using Mean Absolute Error. Finally pick the best performing algorithm. <br>

## Front End
I would like to implement a webpage where it takes information like source and destination from the customer then provides the estimated fare for the trip. <br>

## Cloud Storage
I would like store my data in the S3 bucket of AWS and acces it in my python program. <br>

## Source of Data
I have choosen DC taxi rides dataset available at https://opendata.dc.gov/documents/2b61c28adfbd431587ec728829cceb6e/explore 

## Data Columns

COLUMN_NAME		DATA_TYPE		DESCRIPTION <br>
OBJECTID			NUMBER(9)		Table Unique Identifier	<br>
TRIPTYPE			VARCHAR2(255)	Type of Taxi Trip <br>
PROVIDERNAME		VARCHAR2(255)	Taxi Company that Provided 								trip	<br>
FAREAMOUNT			VARCHAR2(255)	Meter Fare Amount <br>
GRATUITYAMOUNT		VARCHAR2(255)	Tip amount <br>
SURCHARGEAMOUNT		VARCHAR2(255)	Surcharge fee <br>
EXTRAFAREAMOUNT		VARCHAR2(255)	Extra fees <br>
TOLLAMOUNT			VARCHAR2(255)	Toll amount <br>
TOTALAMOUNT		VARCHAR2(255)	Total amount from Meter 								fare, tip, surcharge, 								extras, and tolls. <br>
PAYMENTTYPE		VARCHAR2(255)	Payment type <br>
ORIGINCITY			VARCHAR2(255)	Pick up location city <br>
ORIGINSTATE		VARCHAR2(255)	Pick up location state <br>
ORIGINZIP			VARCHAR2(255)	Pick up location zip <br>
DESTINATIONCITY		VARCHAR2(255)	Drop off location city <br>
DESTINATIONSTATE		VARCHAR2(255)	Drop off location state <br>
DESTINATIONZIP		VARCHAR2(255)	Drop off location zip <br>
MILEAGE			VARCHAR2(255)	Trip milaege <br>
DURATION			VARCHAR2(255)	Trip time - duration of 								travel <br>
ORIGIN_BLOCK_LATITUDE	NUMBER		Pick up location latitude <br>
ORIGIN_BLOCK_LONGITUDE/NUMBER		Pick up location longitude <br>
ORIGIN_BLOCKNAME		VARCHAR2(255)	Pick up location street 								block name <br>
DESTINATION_BLOCK_LAT	NUMBER		Drop off location latitude <br>
DESTINATION_BLOCK_LONGNUMBER		Drop off location longitude <br>
DESTINATION_BLOCKNAME	VARCHAR2(255)	Drop off location street 								block name <br>
AIRPORT			CHAR(1)		Pick up or drop off 									location is a local airport 							(Y/N) <br>
ORIGINDATETIME_TR	DATE			Pick up date and time	 <br>
DESTINATIONDATETIME_TRDATE			Drop off date and time	 <br>

## Additional Information
Payment Type <br>
1.	Credit <br>
2.	Cash <br>
3.	EHail  <br>
4.	Other (not sure how common this is) <br>
5.	Uber (not sure how common this is) <br>

Trip Type <br>
1.	Ordinal (normal rate) <br>
2.	VoD <br>
3.	TransportDC (grant program) <br>
4.	TransportDCShared (grant program) <br>
5.	MOVA (grant program) <br>
6.	CFSA (grant program) <br>
7.	NRS (grant program) <br>
8.	NEMT (grant program <br>

## Feature Selection
My X variables would be PROVIDERNAME, FAREAMOUNT, GRATUITYAMOUNT, SURCHARGEAMOUNT, EXTRAFAREAMOUNT, TOLLAMOUNT, PAYMENTTYPE, ORIGINCITY, ORIGINSTATE, DESTINATIONCITY, DESTINATIONSTATE, MILEAGE, DURATION, ORIGIN_BLOCK_LATITUDE	NUMBER, ORIGIN_BLOCK_LongNUMBER	NUMBER, DESTINATIONDATETIME_TRDATE

My Y variable would be TOTALAMOUNT
