# CTC16-Data-Gathering

The aim of this project is to collected all the airquality sensors in aberdeenshire and present them in a simple to use api. 

This repo uses Python3.

# API V2

## Using the API
See the [Wiki](https://github.com/CodeTheCity/CTC16-Data-Gathering/wiki)

## Run the API locally
The API is currently a python server. You need to run this locally

* Install Python v3
* pip install the following:
    * flask
    * python-dateutil
* run server via commandline "python ./AbdnServer.py"

# API v1

STILL ACTIVE BUT NOT RECOMMENDED. USE API V2.

## Using the API
(server address) /api/v1/data?
* lat
* lon
* id (this is the luftdaten sensor location id, it can be used instead of lat/lon. If given it is used, else lat/lon is used)
* start_date (should be earlier than end_date)
* end_start

Examples: 

http://127.0.0.1:5000/api/v1/data?lat=56.964&lon=-2.212&start_date=2019-05-05T10:00:00&end_date=2019-05-25T11:00:00

http://127.0.0.1:5000/api/v1/data?id=11607&start_date=2019-05-05T10:00:00&end_date=2019-05-25T11:00:00

## Run the API locally
The API is currently a python server. You need to run this locally

* Install Python v3
* pip install the following:
    * flask
    * python-dateutil
* run server via commandline "python ./AbdnServer.py"

This will run the server locally (127.0.0.1) on port 5000.

To access the API open a web browser and naviagte to:

http://127.0.0.1:5000/api/v1/data?lat=56.964&lon=-2.212&start_date=2019-05-05T10:00:00&end_date=2019-05-25T11:00:00