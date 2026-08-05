---
type: lookup
id: esri-shapefile
asset: file-format-software-version-compatibility
title: "ESRI Shapefile — GIS vector format capabilities and limitations in GDAL"
sources:
  - https://gdal.org/en/stable/drivers/vector/shapefile.html
source_quote: "://gdal.org/en/stable/drivers/vector/selafin.html> Previous ESRI Shapefile / DBF  Driver short name ESRI Shapefile Driver built-in by default This driver is built-in by default All varieties of ESRI Shapefiles should be available for reading, creation and editing. The driver can also handle standalone DBF files without associated .shp files. Normally the OG"
generated: true
verified: false
harvested: 2026-08-04
stale_after: 2027-01-31
driver_short_name: "ESRI Shapefile"
format_description: "ESRI Shapefile / DBF"
built_in: "This driver is built-in by default"
write_support: "Supports Create()"
field_name_limit: "up to 10 characters"
supported_field_types: "Only Integer, Integer64, Real, String and Date (not DateTime, just year/month/day) field types are supported. The various list, and binary field types cannot be created."
file_size_limit: "the OGR shapefile implementation has a limitation to 4GB"
key_limitations: "Attribute names can only be up to 10 characters long; ESRI shapefiles can only store one kind of geometry per layer (shapefile); the driver knows to auto-extend string and integer fields (up to the 255 bytes limit imposed by the DBF format)"
unverified_fields: field_name_limit, file_size_limit, key_limitations, supported_field_types, write_support
---
**Driver short name:** ESRI Shapefile

**Format:** ESRI Shapefile / DBF

**Built-in by default:** This driver is built-in by default

**Write support:** Supports Create()

**Field name length limit:** up to 10 characters

**Supported field types:** Only Integer, Integer64, Real, String and Date (not DateTime, just year/month/day) field types are supported. The various list, and binary field types cannot be created.

**File size limit:** the OGR shapefile implementation has a limitation to 4GB

**Key limitations:** Attribute names can only be up to 10 characters long; ESRI shapefiles can only store one kind of geometry per layer (shapefile); the driver knows to auto-extend string and integer fields (up to the 255 bytes limit imposed by the DBF format)

> ://gdal.org/en/stable/drivers/vector/selafin.html> Previous ESRI Shapefile / DBF  Driver short name ESRI Shapefile Driver built-in by default This driver is built-in by default All varieties of ESRI Shapefiles should be available for reading, creation and editing. The driver can also handle standalone DBF files without associated .shp files. Normally the OG

Source: <https://gdal.org/en/stable/drivers/vector/shapefile.html>
