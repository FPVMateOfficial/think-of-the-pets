![Simpson think of the children meme, but children is crossed out and it says "pets"](https://raw.githubusercontent.com/FPVMateOfficial/think-of-the-pets/refs/heads/main/readme_assets/think_of_the_pets_meme.jpg.png)

# What is this?

An opensource GeoJSON file containing polygons of active conflicts throughout the world.

![World map displaying polygons around current conflict areas](https://raw.githubusercontent.com/FPVMateOfficial/think-of-the-pets/refs/heads/main/readme_assets/current_restrictions.png)

# Why?

While developing software for toy helicopters (drones) I realized the need to [geofence](https://en.wikipedia.org/wiki/Geofence) the app; to prevent its usage in combat.
If you're a developer and want to prevent your code from running in the battlefield, this data set is for you.

**You don't want to be the reason someone doesn't come home to their pet.**

# How

1. Using [kepler.gl](https://kepler.gl/) visualize fatalities from the [ACLED (Armed Conflict Location & Event Data)](acleddata.com) data set. Then filter for data points with 10 or more fatalities.
2. Manually create approximate polygons around the high-fatality areas.
3. Copy the polygon data and have ChatGPT convert that into GeoJSON.
4. Add new polygon to our existing GeoJSON

![screenshot of Kepler data tool showing a heat map of fatalities in Eurasia](https://raw.githubusercontent.com/FPVMateOfficial/think-of-the-pets/refs/heads/main/readme_assets/kepler_screenshot.png)

# Contribute

As conflicts begin and end, this data set will need to be updated. If you see any areas that should be add or removed please create a pull request with your changes.

Here's a quick tool to view our edit the GeoJSON data: [uMap link](https://umap.openstreetmap.fr/en/map/anonymous-edit/1144055:UnODy8YK-mvnR_lgeYjGl1PFRnDA8ujtQ1rsShld_jE).
Then export a geojson file and submit a pull request.
