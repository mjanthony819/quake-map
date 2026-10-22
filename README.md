# quake map

Live earthquakes from the USGS, plotted on a world map — circle size is magnitude, color is depth.

**Live demo:** https://mjanthony819.github.io/quake-map/

## what it does

- pulls the free, keyless [USGS GeoJSON feed](https://earthquake.usgs.gov/earthquakes/feed/): past hour / day / week, or significant quakes of the past month
- circle size scales with magnitude; color shows depth (shallow < 70 km, intermediate, deep > 300 km)
- click any circle for time, depth and a link to the USGS event page
- sidebar lists the largest quakes in view — click one to fly to it
- minimum-magnitude filter, auto-refresh every 5 minutes, light/dark basemap

## stack

Single `index.html` — vanilla JS + [Leaflet](https://leafletjs.com/) with OpenStreetMap + Esri basemaps (both free, no API keys). Hosted on GitHub Pages.

## run locally

Open `index.html` in a browser (needs internet for the feed and map tiles).

---

Built with AI assistance (design and direction by [@mjanthony819](https://github.com/mjanthony819)).
