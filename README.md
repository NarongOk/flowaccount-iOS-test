# Search places from Google Map API
- I would like to ​search for places within a specified area.

## Requirement
1 Input
  - Two input parameters are required from user: Geographic coordinates (latitude, longitude) and radius from the given point to define search area.
  - Input can be in any form. Eg. UITextField or UITextArea Map with ability to drop pin and define circular radius, or whatever you find that suits the requirements.
  - Pass Search button
2 Output
  - Display search result information in a ​custom​ UITableView, UITableViewCell.
  - Display search result information in a Map View with custom pin.
  - Table View should be sorted by place name (a-z, A-Z, ก-ฮ)
  - Table View should be display ​Place name​, ​Distance​ from the input geographic coordinate in KM and ​place’s photo ​(if available).

### Implementation Guide
  ■ Update Table View with search results from Google Map API. If search result matched the existing places, not update the record, else add a new record to Table View.
  ■ Place’s image URL can be found in photos -> photo_reference in GG map JSON object
  ■ Custom Table View Cell to display photo, place name and distance.

### Acceptance Criterias
  ■ App should be written in Swift 3++.
  ■ Architecturing your code wisely: for example, using VIPER, Clean Architecturing, MVVM.
  ■ Photo loading should be asynchronous.
  ■ You are required to ​submit your​ well documented source code to this GITHub repository

## Google Map API 
  - URL: https://maps.googleapis.com/maps/api/place/nearbysearch/json?location=18.7717874,98.9742796&radius=1500&key=AIzaSyBIq36Frxw21zxMvU49jOMZ40wpvtYsC68
  - Method: POST
  - location: The latitude/longitude around which to retrieve place information
  - radius: Defines the distance (in meters) maximum radius 50000 meters
  - key: you can use this key: ​"AIzaSyBIq36Frxw21zxMvU49jOMZ40wpvtYsC68"
