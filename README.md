# Google Api #

### What is this repository for? ###

* Google Api Tutorial
* https://developers.google.com/maps/documentation/javascript/tutorial

### How do I get set up? ###

* This example creates a Google Map in HTML:
  Example
	<!DOCTYPE html>
	<html>
		<body>

			<h1>My First Google Map</h1>

			<div id="googleMap" style="width:100%;height:400px;"></div>

			<script>
				function myMap() {
					var mapProp= {
    					center:new google.maps.LatLng(51.508742,-0.120850),
    					zoom:5,
					};
					var map=new google.maps.Map(document.getElementById("googleMap"),mapProp);
				}
			</script>

			<script src="https://maps.googleapis.com/maps/api/js?key=YOUR_KEY&callback=myMap"></script>

		</body>
	</html>
	
* Map Setup

1.The Map Container and Size
  The map needs an HTML element to hold the map:

		<div id="googleMap" style="width:100%;height:400px"></div>
		
2.Create a Function to Set The Map Properties
  
  		function myMap() {
			var mapProp= {
    			center:new google.maps.LatLng(51.508742,-0.120850),
    			zoom:5,
				};
			var map=new google.maps.Map(document.getElementById("googleMap"),mapProp);
			}
			
  The mapProp variable defines the properties for the map.

  The center property specifies where to center the map (using latitude and longitude coordinates).

  The zoom property specifies the zoom level for the map (try to experiment with the zoom level).

  The line: var map=new google.maps.Map(document.getElementById("googleMap"), mapProp); creates a new map inside the <div> element with id="googleMap", using the parameters that are passed (mapProp).

3.Free Google API Key
  Google allows a website to call any Google API for free, thousands of times a day.

  Go to https://console.developers.google.com to get a free API key.

  Google Maps expects to find the API key in the key parameter when loading an API:

<script src="https://maps.googleapis.com/maps/api/js?key=YOUR_KEY&callback=myMap"></script>

### Example ###
* This example creates a Google Map centered in London, England:

	<!DOCTYPE html>
	<html>
		<body>

			<h1>My First Google Map</h1>

			<div id="googleMap" style="width:100%;height:400px;"></div>

			<script>
				function myMap() {
					var mapProp= {
    					center:new google.maps.LatLng(51.508742,-0.120850),
    					zoom:5,
					};
					var map=new google.maps.Map(document.getElementById("googleMap"),mapProp);
				}
			</script>

			<script src="https://maps.googleapis.com/maps/api/js?key=YOUR_KEY&callback=myMap"></script>

		</body>
	</html>
	
### Who do I talk to? ###

* Mitesh Banka
  banka.mitesh@gmail.com
  +91-8482096370