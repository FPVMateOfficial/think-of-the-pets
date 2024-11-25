# What is this?

An opensource GeoJSON file containing polygons of active conflicts throughout the world.

# Why?

While developing software for toy helicopters (drones) I realized the need to [geofence](https://en.wikipedia.org/wiki/Geofence) the app; to prevent its usage in combat.
If you're a developer and want to prevent your code from running in the battlefield, this data set is for you.

**You don't want to be the reason someone doesn't come home to their pet.**

# How

1. Using [kepler.gl](https://kepler.gl/) visualize fatalities from the [ACLED (Armed Conflict Location & Event Data)](acleddata.com) data set. Then filter for data points with 10 or more fatalities.
2. Manually create approximate polygons around the high-fatality areas.
3. Copy the polygon data and have ChatGPT convert that into GeoJSON.
4. Add new polygon to our existing GeoJSON

![screenshot of Kepler data tool showing a heat map of fatalities in Eurasia](https://github.com/FPVMateOfficial/think-of-the-pets/TODO)

# Contribute

As conflicts begin and end, this data set will need to be updated. If you see any areas that should be add or removed please create a pull request with your changes.

TODO: https://geojson.tools/ link
