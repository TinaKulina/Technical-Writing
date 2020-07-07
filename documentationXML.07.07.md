**exercises form "Learn API Technical Writing: JSON and XML for Writers" Udemy **

##### Request to record a TV program

||||||
|--- |--- |--- |--- |--- |
|element|description|type|required|notes|
|recordtv|data on when a tv program is to be recorded|tv program data|required||
|date|the date when the program starts|string|optional|format is yyyy-mm-dd.Valid value: today's date|
|time|the time the program starts|string|required|attributes: format has values "24" or "12" for 24 or 12 hour formats|
|duration|the length of the program|number|required|format is hh:mm, with am or pm afterwards for 12 hour format|
|station|the channel where the program is for record|number|required|in hours|

   
 #####  Different TV request
 

|||||||
|--- |--- |--- |--- |--- |--- |
|element|attribute|description|type|required|note|
|recordtv||data on when a tv program should be recorded|tv program data|required||
|when||the date and time when the program starts|date and time data|required||
||date|the date|string|optional|date in yyyy-mmdd format. default value is today's date.|
||time|the time the program begins|string|required|format is hh:mm, with am or pm afterwards for 12 hour format|
||format|the format for the time:either 12 hour or 24 hour|number|required|valid values: 24, 12|
|duration||the length of the program|number data|required||
||hours|the length of the program in hours|number|required||
|station||the station to record|station data|required||
||channel|the channel|number|required||



#####  Temperature and Humidity

  **Top level**

| Element                  | Description                                        |   Type             |  
|-------------------------:|:--------------------------------------------------:|:------------------:|
| dailyData                |  Temperature and humidity data for one day         | dailyData element  |




 **dailyData: Represents temperature and humidity data for one day**
 

 
| Element         | Description                                     | Type                 |   Notes             |        
|:---------------:|:-----------------------------------------------:|:--------------------:|:-------------------:|
| date            | The date when the device was read               | string               |  Format: YYYY-MM-DD |
| hourlyData      | Temperature and humidity data for one hour      | hourlyData element   |                     |



 **hourlyData: Represents temperature and humidity data for one hour**  
  
  
  
| Element         | Description                         | Type            |   Notes         |  
|----------------:|:-----------------------------------:|:---------------:|:---------------:|
| time            | The time  the temperature was taken | string          |  Format: HH:MM  |
| device          | device objects with data            | device element  |                 | 



 **device: Contains temperature and humidity data from a device**
  
| Element           | Description                                       |   Type    | 
|------------------:|:-------------------------------------------------:|:---------:|
| id                |  The device's ID                                  |  number   |
| temperature       |  The measured temperature in degrees Fahrenheit.  |  number   |
| humidity          |  The measured humidity in percentage              |  number   |


  
