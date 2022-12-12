# Fennorad Mapbox

## Introduction
This is a library that forks [BlazorMapbox](https://github.com/johnsonea2/BlazorMapbox) with some enhancements. This adds [Directions](https://github.com/mapbox/mapbox-gl-directions) and geolocation components to the library. 

## Getting Started
### Prerequisites & Installation 
---
- Your application needs to target .NET 6.
- A Mapbox access token is required to view the map. You can acquire one at https://account.mapbox.com/access-tokens/. 

### Usage 
---
- Add a using statement of `@using Blazor.Mapbox` to the top of your page. 
- Add the component anywhere in the markup similar to: 
```
<MapboxMap AccessToken="{YOUR ACCESS TOKEN HERE}"></MapboxMap>
```
- In order to add directions and/or geolocation ensure you add
```
<MapboxMap AccessToken=@AccessToken AddDirectionsFlag=@true AddGeoLocationFlag=@true></MapboxMap>
```


- In order for this package to work with a deployable you need to add the following script to your `_Host.cshtml`
```
<script src="~/_content/Fennorad.Mapbox/MapboxInterop.js"></script>
```

