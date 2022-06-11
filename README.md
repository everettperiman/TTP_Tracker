# TTP_Tracker
Used to track TTP appointments


## URL A
This url is used to lookup any data that one could desire. In the example url used here it contains a location id to search by.
https://ttp.cbp.dhs.gov/schedulerapi/locations/5444/slots?

### Options
startTimestamp=YYYY-MM-DDTHH:MM:SS
endTimestamp=YYYY-MM-DDTHH:MM:SS


## URL B
https://ttp.cbp.dhs.gov/schedulerapi/slots?

## URL C
https://ttp.cbp.dhs.gov/schedulerapi/slots/asLocations

### Options
minimum=1-10
This is the minimum number of appts that should be available for that location. Useful if wanting to enroll families at one time.

filterTimestampBy=before|on
This constrains the results to show if they appear ON the searched date or BEFORE the search date.

serviceName=Global%20Entry
This sets the searched service, leave blank to see all programs.

timestamp=YYYY-MM-DD
Sets the desired timestamp to search BY or ON.

### Examples
Searching for all appts by specific date at all locations for Global Entry with at least 1 open appt.
minimum=1&filterTimestampBy=before&timestamp=2022-07-01&serviceName=Global%20Entry

Searching for all appts on a specific data for all Locations for Global Entry with at least 2 open appts.
minimum=1&filterTimestampBy=on&timestamp=2022-06-30&serviceName=Global%20Entry

