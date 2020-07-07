exercises form "Learn API Technical Writing: JSON and XML for Writers" Udemy 

##### Request to record a TV program
| Element         | Description                                   |Required   | Type           | Notes                                                                                                                                |
|:---------------:|:----------------------------------------------|----------:|:--------------:|:------------------------------------------------------------------------------------------------------------------------------------:|
| recordTV        | Data on when a TV program should be recorded  | Required  |TV program data |                                                                                                                                      |
|      | date     | The date when the program is to be recorded   | Optional  | string         | Format is YYYY-MM-DD.Valid value: today's date                                                                                       |
|      | time     | The time the program starts                   | Required  | string         | Attributes: format has values "24" or "12" for 24 or 12 hour formats. Format is HH:MM, with am or pm afterwards for 12 hour format.  |
|      | duration | The length of the program                     | Required  | number         |  in hours                                                                                                                            |
|      | channel  | The channel where the program is for record   | Required  | number         |                                                                                                                                      |
   
   
 #####  Different TV request
 
| Element         | Attribute        | Description                                        |   Type             | Required   |  Notes 
|:---------------:|:----------------:|:--------------------------------------------------:|:------------------:|:----------:|:------------------------------------------------------------|  
| recordTV        |                  | Data on when a TV program should be recorded       | TV program data    | Required   |  
|      |   when   |                  | The date and time when the program starts          | Date and time data | Required   |
|      |          |      date        | The date                                           | string             | Optional   | Date in YYYY-MMDD format. Default value is today's date.   
|      |          |      time        | The time the program starts                        | string             | Required   | Format is HH:MM, with am or pm afterwards for 12 hour format.
|      |          |     format       | The format for the time: either 12 hour or 24 hour | number             | Required   | Valid values: 24, 12
|      | duration |                  | The length of the program                          | number             | Required   |  
|      |          |     hours        | The length of the program in hours                 | number             | Required   |
|      | station  |                  | The station to record                              | Station data       | Required   |
|      |          |     channel      | The channel                                        | number             | Required   |


#####  Temperature and Humidity

  Top level

| Element                  | Description                                        |   Type             | 
|:------------------------:|:--------------------------------------------------:|:------------------:|:
| dailyData                |  Temperature and humidity data for one day         | dailyData element  |


  dailyData: Represents temperature and humidity data for one day
  
| Element         | Description                                     | Type                 |   Notes             |        
|:---------------:|:-----------------------------------------------:|:--------------------:|:-------------------:|
| date            | The date when the device was read               | string               |  Format: YYYY-MM-DD |
| hourlyData      | Temperature and humidity data for one hour      | hourlyData element   |                     |


  hourlyData: Represents temperature and humidity data for one hour
  
| Element         | Description                                     | Type                 |   Notes             |                                                                                                                       |
|:---------------:|:-----------------------------------------------:|:--------------------:|:-------------------:|
| time            | The time  the temperature was taken             | string               |  Format: HH:MM      |
| device          | device objects with data                        | device element       |                     | 



  device: Contains temperature and humidity data from a device
  
| Element           | Description                                       |   Type    | 
|:-----------------:|:-------------------------------------------------:|:---------:|:
| id                |  The device's ID                                  |  number   |
| temperature       |  The measured temperature in degrees Fahrenheit.  |  number   |
| humidity          |  The measured humidity in percentage              |  number   |

  
  