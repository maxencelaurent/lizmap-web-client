# Changelog Lizmap 3.8

<!--
Format from https://keepachangelog.com/en/1.0.0/
added, fixed, changed, removed, deprecated, security
with some extra keywords: backend, tests, test, translation, funders, important
-->

## Unreleased

## 3.8.0-rc.1 - 2024-06-06

### Added

* New JavaScript API to load external layer straight in the legend tree and in the map
* Popup: FeatureToolbar in compact table
* Review of the **tooltip** feature using the new version of the plugin

### Removed

* Zoom history
* Unused button about the layer extent

### Fixed

* Handle baselayers visibility in theme
* Popup was not shown in the **Atlas** container
* Let min/max resolutions be handled by OpenLayers for WMTS
* Drawing tool : keep draw visible when closing minidock
* Dataviz in popup generate two feature toolbar in parent popup
* Apply min and max resolutions to base layers removed by single WMS Layer
* More fixes about XSS
* Tooltip :
  * Don't show tooltip tool when device has coarse pointer
  * Remove legacy code
  * Handle linestring layers
* Fix loading GIF about Lizmap being transformed about color
* Refresh the layer after editing when using the "single WMS tile mode"

### Backend

* New `lizmap-message` component
* Defer JavaScript scripts loading
* Refactoring of Web Components, about OpenLayers
* Review the way to load JavaScript
* Review ESLint configuration
* Upgrade Jelix to 1.8.9
* Upgrade OpenLayers to 9.2.3

## 3.8.0-alpha.1 - 2024-03-21

### Added

* Load layers as a single WMS layer, contribution from @mind84
* Improve snapping functionalities, contribution from @mind84
* New management of the N to M relations data editor, contribution from @mind84
* Display features at startup when set in URL
* Improvement on the landing page HTML content (logged and not logged user)

### Removed

* Buttons about zoom history

### Backend

* Some JavaScript and PHP refactoring, code cleaning
* Update OpenLayers to version 9
* Improve migration to OpenLayers 9
  * OL 9 map on top now
  * Popup
  * Locate by layer highlight

### Translations

* Update translated strings from the Transifex website :
  * [Lizmap Web Client](https://www.transifex.com/3liz-1/lizmap-locales/dashboard/)
  * [Jelix](https://www.transifex.com/3liz-1/jelix/dashboard/)

### Funders

* **[Faunalia](https://www.faunalia.eu/fr)**, contributions on source code from @mind84
* **[JPEE](https://www.jpee.fr/)**
