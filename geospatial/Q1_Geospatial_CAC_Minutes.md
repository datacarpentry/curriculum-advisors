Geospatial Curriculum Advisory Committee

Q1 Meeting March 30, 2022 16:00 UTC

Minutes

**Attendees**

- Stephen Appel
- Jeff Hollister
- Justin Fain
- Mike Mahoney
- Erin Becker

**New Business**

1. Transition from PROJ and proj4strings
    * Lessons should be updated to reference coordinate systems by their EPSG codes from the EPSG Geodetic Parameter Dataset instead of using proj4strings. The Committee agreed that the alternative Well-known text (WKT) representation is unwieldy and unnecessary for most common use cases. WKT should be mentioned as an alternative to EPSG codes, especially where there is no existing EPSG standard. Lessons should include examples of converting between the EPSG and WKT representations.
2. Deprecation of the sp, rgeos, and rgdal packages
    * The Committee agreed that the references to rgdal and rgeos be removed or replaced with references to the equivalent sf and terra functions as appropriate. This decision is closely paired with the rationale for choosing terra as the replacement for the raster package and aims to avoid code-breaking deprecations coming some time in 2023.
3. Transition from raster to terra or stars
    * The terra package appears to be the most direct replacement for raster as it uses language which is similar to raster and common to other GIS. The Committee recommends that terra be adopted as a replacement to raster. Stars should be presented as an alternative to terra that may be faster in some cases or more appropriate for analyses with longitudinal elements.
