# Journey

A lightweight, URL-driven world map for places and dates. It is a standalone static site built with HTML, CSS, and vanilla JavaScript; no build step, API key, or backend is required.

## Events

Open the site with a `places` query parameter. Each event has the format `City|YYYY-MM`; separate events with semicolons:

```text
?places=City%7CYYYY-MM%3BCity%7CYYYY-MM
```

Replace the placeholders with the places and dates to display. The city names and dates are read from the URL and are not stored in the page. Spaces and non-ASCII characters can be URL-encoded, for example `Los%20Angeles` or `D%C3%BCsseldorf`.

Coordinates for supported cities are technical map data stored in `locations.json`; the file contains no event dates. Cities without coordinates are skipped.

## Map source

`assets/world-map.svg` is based on [BlankMap-World-Equirectangular.svg](https://commons.wikimedia.org/wiki/File:BlankMap-World-Equirectangular.svg)
