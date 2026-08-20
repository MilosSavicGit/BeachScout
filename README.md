# BeachScout

**Part of ScoutPlatform**

BeachScout is a browser-based and Android-compatible geospatial
application for discovering beaches, naturist beaches, naturist resorts,
campsites and swimming locations around the world.

BeachScout is the first production application built on
**ScoutPlatform**, a family of lightweight exploration tools designed to
help people **discover, document and share knowledge about places**
using open geographic resources.

------------------------------------------------------------------------

# Overview

Unlike a conventional map, BeachScout performs live semantic searches
around a selected location, enriches results from multiple open data
sources and allows visitors to contribute photographs and local
knowledge.

The application is designed to remain lightweight while providing
worldwide coverage.

------------------------------------------------------------------------

# Features

-   Worldwide place search
-   Predictive country search
-   Predictive place search
-   Current location search
-   10 km local searches
-   Numbered beach markers
-   Official and customary naturist beaches
-   Naturist resorts and campsites
-   Country-wide naturist and dog beach browsing
-   Live beach conditions and recommendation
-   Accommodation within 3 km of a beach
-   Nearest public parking
-   Google Maps integration
-   Wikipedia / Wikimedia links
-   Community photo uploads
-   Community descriptions
-   Community place suggestions
-   Moderation workflow
-   Translation and transliteration
-   Android compatible
-   Supabase analytics

------------------------------------------------------------------------

# Technology Stack

## Front End

-   HTML5
-   CSS3
-   Vanilla JavaScript (ES6)

Single Page Application (SPA)

## Mapping

-   MapLibre GL JS
-   OpenFreeMap (streets basemap — keyless OSM vector tiles, Liberty style)
-   Esri World Imagery (satellite basemap — keyless)
-   OpenStreetMap (map data)

Both basemaps are keyless, so there is no vendor account, no API key in
the source, and no monthly request or session limit to exhaust.

## Search

-   Photon (search-as-you-type, typo tolerant)
-   Nominatim (fallback and reverse geocoding)
-   Overpass API

## Conditions

-   Open-Meteo forecast API (air temperature, wind, UV, rain, sunset)
-   Open-Meteo marine API (sea temperature, wave height)

## Database

-   Supabase

Used for:

-   Analytics
-   Community photographs
-   Community descriptions
-   Moderation

------------------------------------------------------------------------

# Open Data Sources

-   OpenStreetMap
-   OpenMapTiles
-   OpenFreeMap
-   Overpass API
-   Photon
-   Nominatim
-   Open-Meteo
-   Wikimedia Commons
-   Wikipedia
-   Wikidata
-   Supabase

------------------------------------------------------------------------

# Attribution

Map data © OpenStreetMap contributors, available under the
[Open Database License](https://www.openstreetmap.org/copyright).

**Street basemap** — vector tiles from [OpenFreeMap](https://openfreemap.org),
Liberty style, using the [OpenMapTiles](https://openmaptiles.org) schema.
OpenFreeMap is a free public instance funded by donations, with no API
keys and no request limits.

**Satellite imagery** — Esri World Imagery: Esri, Maxar, Earthstar
Geographics.

**Rendering** — [MapLibre GL JS](https://maplibre.org), BSD 3-Clause.

**Place search** — [Photon](https://photon.komoot.io) by Komoot, with
[Nominatim](https://nominatim.openstreetmap.org) (OpenStreetMap
Foundation) as fallback and for reverse geocoding.

**Beach and accommodation data** — [Overpass API](https://overpass-api.de),
served by community mirrors including private.coffee, VK Maps and FOSSGIS.

**Weather and marine data** — [Open-Meteo](https://open-meteo.com),
CC BY 4.0. Sea temperature and wave height are modelled, not measured at
the beach.

**Photographs** — [Wikimedia Commons](https://commons.wikimedia.org) and
[Wikidata](https://www.wikidata.org), under their respective licences.

Basemap attribution is rendered in-app in the corner of the map via
MapLibre's attribution control.

------------------------------------------------------------------------

# Design Philosophy

BeachScout intentionally avoids downloading large regional datasets.

Workflow:

1.  Select a place
2.  Perform a live 10 km search
3.  Display nearby beaches and related locations

This keeps the application lightweight while always working with current
OpenStreetMap information.

------------------------------------------------------------------------

# Data Caveats

OpenStreetMap coverage is uneven, and BeachScout says so rather than
papering over it:

-   **Dog access** is recorded on under 2% of beaches. Absence of a tag
    is not a statement either way. Germany is best covered at around 5%;
    some countries have none at all.
-   **Naturist status** distinguishes officially designated places from
    those where naturism is merely customary or tolerated. Places
    identified as naturist by name alone carry no tag and are labelled
    as such.
-   **Inland versus coastal** is a heuristic. OpenStreetMap tags a
    lakeside beach exactly like a sea beach.
-   **Sea temperature and waves** have no coverage on lakes and rivers,
    which is a large share of the dataset.

Local rules change, particularly with the season. Check local signs.

------------------------------------------------------------------------

# Geographic Naming

Certain territories are included to make searching easier. Their
inclusion and naming are intended solely to help users find places and
do not imply a political position by BeachScout or ScoutPlatform.

------------------------------------------------------------------------

# ScoutPlatform

BeachScout is one of the core ScoutPlatform applications.

## Current applications

-   🏖 BeachScout
-   🛣 RoadScout

## Planned applications

-   ⛰ MountainScout
-   🏛 HeritageScout
-   🌊 LakeScout
-   🕳 CaveScout
-   🐦 BirdScout

The ScoutPlatform engine provides:

-   Interactive maps
-   Predictive search
-   Community photographs
-   Community descriptions
-   Moderation
-   Translation
-   Analytics

------------------------------------------------------------------------

# Contribution to Open Knowledge

BeachScout complements projects such as OpenStreetMap, Wikipedia and
Wikimedia Commons by encouraging visitors to contribute:

-   Original geotagged photographs
-   Multilingual local descriptions
-   Beach access information
-   Parking information
-   Missing geographic knowledge

Corrections to the underlying map data are best made directly in
[OpenStreetMap](https://www.openstreetmap.org) — they then reach
BeachScout and every other OSM-based application at the next data
regeneration.

User-submitted photographs and descriptions remain the property of their
contributors. BeachScout receives permission only to store, moderate and
display them as part of the service.

------------------------------------------------------------------------

# Current Status

**Version:** 2.3.5

-   Browser: Stable
-   Android: Stable
-   Worldwide search: Implemented
-   Country-wide browsing: Implemented
-   Beach conditions: Implemented
-   Community uploads: Implemented
-   Moderation: Implemented
-   Translation: Implemented

------------------------------------------------------------------------

# Created by

**Milos Savic**

Belgrade, Serbia

BeachScout is developed as part of **ScoutPlatform**, whose mission is
to build lightweight, community-powered applications for discovering,
documenting and preserving knowledge about places around the world.

🌐 **Website:** [bymilossavic.com](https://bymilossavic.com)
contact@bymilossavic.com
