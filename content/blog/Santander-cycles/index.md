---
title: Santander Cycles Locator
date: "2025-05-01"
description: Project built to locate Santander cycles and its stations in London, UK.
---

#Santander Cycles Locator

This was one of the first projects that I built combining two API's: I used Google Maps and TfL's API.
This shows a map of London and all the locations of the Santander Cycles docking stations and the distance from your current location to the closest one.

> Santander Cycles is a public bicycle hire scheme in London, Swansea and Milton Keynes United Kingdom. The scheme's bicycles are popularly known as Boris Bikes, after Boris Johnson, who was the Mayor of London when the scheme was launched. The operation of the scheme is contracted by Transport for London to Serco.

```javascript
if (availableBikes > 0) {
  if (!closestInfoWindow || distance < closestDistance) {
    closestInfoWindow = infoWindow
    closestDistance = distance
    closestMarker = marker
  }
}
```

if we're the first window we've found, or if our distance is smaller than the previously closest, then set this as the closest one
