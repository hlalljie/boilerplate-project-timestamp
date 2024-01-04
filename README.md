# Timestamp Microservice

This microservice prints out the the Unix time in milliseconds and the GMT 0 time string.  

To query the api you will type in the url followed by /api/`your query here` and one of the options below:
1. Leave black after `url`/api/ to get the current time
2. Type in a date string in a format readable by Javascript Date function. F.e. url/api/August 19, 1975 23:15:30 would return:  
{"unix":177747330000,"utc":"Wed, 20 Aug 1975 06:15:30 GMT"}  
*Note:Spaces and other date strings should be converted by most browsers to a string compatible with the get function. The above datestring coverts to 'August%2019,%201975%2023:15:30'*

3. Type in a Unix timestamp to get the date. F.e. 1451001600000 would return:  
{ unix: 1451001600000, utc: "Fri, 25 Dec 2015 00:00:00 GMT" }

