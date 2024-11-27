![Simpson think of the children meme, but "children" is crossed out and replaced with "pets"](https://raw.githubusercontent.com/FPVMateOfficial/think-of-the-pets/refs/heads/main/readme_assets/think_of_the_pets_meme.jpg)

# What is this?

An open-source GeoJSON file containing polygons of active conflicts throughout the world.

![World map displaying polygons around current conflict areas](https://raw.githubusercontent.com/FPVMateOfficial/think-of-the-pets/refs/heads/main/readme_assets/current_restrictions.png)

View the [current uMap](http://u.osmfr.org/m/1144487/).

# Why?

While developing software for toy helicopters (drones), I realized the need to [geofence](https://en.wikipedia.org/wiki/Geofence) the app to prevent its usage in combat.

If you're a developer and want to prevent your code from being used on the battlefield, this dataset is for you.

**You don't want to be the reason someone doesn't come home to their pet.**

# How

1. Use [kepler.gl](https://kepler.gl/) to visualize fatalities from the [ACLED (Armed Conflict Location & Event Data)](https://acleddata.com) dataset. Then, filter for data points with 10 or more fatalities.

2. Manually create approximate polygons around high-fatality areas.

3. Copy the polygon data and have ChatGPT convert it into GeoJSON.

4. Add the new polygon to the existing GeoJSON.

![Screenshot of Kepler data tool showing a heat map of fatalities in Eurasia](https://raw.githubusercontent.com/FPVMateOfficial/think-of-the-pets/refs/heads/main/readme_assets/kepler_screenshot.png)

# Contribute

As conflicts begin and end, the dataset will need to be updated. If you see any locations that should be added or removed, please create a pull request with your changes.

We recommend using [uMap](https://umap.openstreetmap.fr/en/):

1. In the bottom right of uMap, there is an import button that accepts a URL.
2. Input the raw data URL for the current GeoJSON file:  
   `https://raw.githubusercontent.com/FPVMateOfficial/think-of-the-pets/refs/heads/main/think-of-the-pets.geojson`
3. Modify the polygons as needed.
4. Export the updated GeoJSON file and submit a pull request.
