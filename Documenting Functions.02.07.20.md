###### Documenting Functions

##safeMode(enable)

Whether to enable safe mode. 

**Parameters:**

   • <strong>enable</strong>

   Type: Boolean

   true to enable safe mode; false to disable safe mode. 


##getPremiumMode()

Whether the user has paid for premium mode. 

**Returns:**

   Type: Boolean

   true if the user has paid for premium mode; false if he has not

##setTimeout(timeout)

Sets the time to wait for a response before timing out. 

**Parameters:**

   • <strong>timeout</strong>

   Type: Number

   Time to wait for a response before timing out. The parameter value is in milliseconds. 

##newEvent(calendarId)

Creates a new event for the specified calendar.

**Parameters:**

   • <strong>calendarId</strong>

   Type: Number

   The ID of the specified calendar

**Returns:**

   Type: Number

   Returns the ID for the new event.

##getDirections(latitude, longitude, directionsCallback)

Returns the directions from the current location to the destination
location.

**Parameters:**

   • <strong>latitude</strong>

   Type: Number

   Latitude of the destination. The parameter value is in degrees

   • <strong>longitude</strong>

   Type: Number

   Longitude of the destination. The parameter value is in degrees.

   • <strong>directionsCallback</strong>

   Type: Functions

   Called when the directions come back from the server. Contains a String parameter
named directions, which has the directions on how to get from the current location to
the destination location.


##createTransaction(amount)
Creates a new transaction.

**Parameters:**

   • <strong>amount</strong>

   Type: Number

   Amount of the transaction. The parameter value is in the default currency

**Returns:**

   Type: String

   Returns the new transaction ID
   
