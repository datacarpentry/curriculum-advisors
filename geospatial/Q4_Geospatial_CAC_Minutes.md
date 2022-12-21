# Geospatial Curriculum Advisory Committee Q4 Meeting Minutes: 

November 29, 2022 20:00 UTC

## Attendees

- Stephen Appel
- Jeff Hollister
- Justin Fain
- Mike Mahoney
- Toby Hodges (Curriculum core team)
- Ryan Avery (Guest)

## Old Business

### Q1 Minutes

Last meeting (3/30/22) minutes here: https://github.com/datacarpentry/curriculum-advisors/blob/main/geospatial/Q1_Geospatial_CAC_Minutes.md   

### Recommendations RE: PROJ, Proj4, sp, rgeos, and rgdal

See [Issue #368](https://github.com/datacarpentry/r-raster-vector-geospatial/issues/368)

Recommendations:

- Transition from PROJ and proj4strings
- Deprecation of the sp, rgeos, and rgdal packages
- Transition from raster to terra or stars
- Relevant Issues:
    - https://github.com/datacarpentry/r-raster-vector-geospatial/issues/364
    - https://github.com/datacarpentry/r-raster-vector-geospatial/issues/363 
    - No relevant PRs
- Action - Engage with those we know are teaching the lessons.
- Action - Draft a blog post to raise awareness of the issue with the wider community, call for volunteers to make the updates
- Blog post template: ​​https://docs.google.com/document/d/12sGIQeNVY5ln6Y-nmDQllZpnl6Qo0CeQaBZA94f0Ggo/edit or https://codimd.carpentries.org/blog-post-template?edit if you prefer
- Tag Toby on the document/share the link by email if you need help.

## New Business

### Geospatial Python

Ryan Avery came as a guest to discuss his work on Geospatial Python.

Links:

* https://carpentries-incubator.github.io/geospatial-python/ 
* https://github.com/carpentries-incubator/geospatial-python
* Recorded workshop: https://youtu.be/Ce7GuGIf3r0 

Currently in Beta - being taught by instructors who are connected to NASA/Ryan.

Info from Ryan:

* 3 years in the making
* Originally started with Ryan's NASA internship.
* Student interns who were new to python but had Geospatial experience
* Introduction to Geo python packages for reading (especially satellite imagery)
* Working with sat. imagery with vector data
* Essentially forked form the R geospatial lesson
* Netherlands e-sciences center and Ryan refactored the lesson and moved away from NEON and highlight python strengths
* Cloud hosted datasets (limitations, advantages)
* The lessons are done and the web pages are cleaned up.
* Enough to teach a full one day+ workshop
* Maptime Davis - heavily attended (see recorded workshop link above)
* Esciences center taught an in-person workshop.

Questions for discussion:

* Since the introductory episodes of the lesson are nearly the same as the R version, what would the workshop webpage look like? [Current webpage](https://datacarpentry.org/geospatial-workshop/).
* What are the implications of two tracks for the same curriculum? Especially if they use different data.
* Should there be two versions of the *Introduction to Geospatial Concepts* lesson or should the two tracks share that curriculum?
* Do people find the multiple lessons confusing on the current curriculum? 
* Should the [*r intro geospatial*](https://datacarpentry.org/r-intro-geospatial/) lesson be eliminated? It's rarely taught.

Toby would like to see the python version taught outside the US by an unaffiliated organization before moving out of beta.

### Workbench Beta

See [issue #369](https://github.com/datacarpentry/r-raster-vector-geospatial/issues/369)

### Issues for next meeting:

* [Removing Factors](https://github.com/datacarpentry/r-intro-geospatial/issues/119)
    * it's been ~3 years since R4.0 deprecated stringsAsFactors, and the option is going to be removed entirely in R 4.3 (https://cran.r-project.org/doc/manuals/r-devel/NEWS.html).
* How will the python version be incorporated into the Geospatial Workshop?
* Blog post about recruiting help for making updates to r-raster-vector-geospatial



