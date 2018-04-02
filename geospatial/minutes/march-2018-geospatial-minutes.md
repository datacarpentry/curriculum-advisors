### March 2018 Meeting of the Geospatial Curriculum Advisors

There were two meetings held:
- Monday, March 26, 2018 at 16:00:00 UTC
- Thursday, March 29, 2018 at 20:00:00 UTC

Attending (meeting one):
- Erin Becker
- Joe Stachelek
- Jeff Hollister
- Chris Prener
- Leah Wasser
- Arthur Endsley
- Anne Fouilloux

Attending (meeting two):
- Erin Becker
- Michele Tobias
- Stace Maples
- Leah Wasser
- Chris Prener
- Anne Fouilloux

Detailed Agenda: https://docs.google.com/document/d/1VG34gKSzQZg-wrvAuDSp-ExCnVZamc6AcAvfzTsemUc

* Megan Jones - unfortunately my schedule is precluding me from attending both meetings. However, I'm happy to answer questions about NEON data.  We are pulling together an updated data set including the SJER & HARV sites for other teaching materials. I'd be happy to share that data with the group if it is desired. 

1) Plotting systems
Static plotting:
- Deciding between base R / ggplot / tmap for teaching static plotting. 
- ggplot support for sf objects (geom_sf) is only available on the development branch. There are major installation issues with working 
from the development branch, and issues around stability. Can avoid working on the development branch by converting sf objects to 
a dataframe (recast) and using the stable version of ggplot. Goal to convert the lesson to geom_sf once it is available in CRAN.
- base R takes a long time to teach because of the difficulty of customizing objects in the plot. 
- tmap is becoming more popular, but is relatively new and no one on the committee has taught with it. More similar to map layout of 
arcGIS. If you're used to GIS, it is more familiar. Could develop an optional hour-long lesson on cartography using tmap. 

Decision: 
- Teach static plotting with ggplot by reading in the data as sf, recasting it to a dataframe and using the stable ggplot on CRAN.
- Lessons are currently in sf. Need to add one function to recast to dataframe and then whatever geoms you want to teach. 
- Convert to the geom_sf when it's stable. 
- Keep an eye on tmap for future updates of the lesson.
- (Potentially) develop a short optional lesson using tmap for cartography.

2) Interactive plotting: 
- Deciding between leaflet / mapview
- Mapview isn't meant to be customized. It makes nice easy graphics but if you want to customize things, leaflet is better. 
- Mapview is useful when the map isn't the endpoint, but when it helps you visualize the analysis. Exploratory.
- Mapview makes a lot of assumptions about what you want the map to look like. Harder to customize but easier to get started.
- Choice depends on our goal. If the goal is to teach people how to make their own interactive maps (e.g. with geoscientists), leaflet makes sense. 
If the goal is to quickly vizualize something and do analysis, mapview. 
- Possible to teach leaflet with only three functions. Possible to get something functional with only a few lines of leaflet. 
- Some opposition to leaflet due to complexity. 
- Mapview outputs a leaflet object. Would be possible to use mapview to generate a leaflet object. Could then pull it out and customize it. 

Decision: 
- Six of eight CAC members voiced support for using leaflet. Keep syntax relatively simple. Leah has a sample lesson teaching leaflet that she will contribute to the Maintainers for them to use as a resource for developing this part of the lesson.

3) Learner level
- Currently lessons don't include any introduction to R. Instructors have been teaching ad hoc introductions to R. Some audiences need the
background and some don't. 
- Don't want to spend too long on intro but can add an introductory lesson to avoid the need to ad lib and make it easier for instructors
to teach the lessons. 
- Can skip the introduction to R if learners have programming experience. 
- Can use the introduction to R lessons from the r-gapminder-novice lessons for SWC. Can tie these data into geospatial and get a 
global perspective. 
- The lessons currently are a mix of teaching geospatial concepts and teaching how to implement geospatial analyses in R. Can pull out some of the introductory concepts (data formats, project organization) from http://www.datacarpentry.org/r-spatial-data-management-intro/ and make them their own repo/lesson. Needs a lot of restructuring. 

Decision:
- Use the r-novice-gapminder lessons as a basis for creating an introduction to R for geospatial. 
- Copy over these lessons and start modification. 

Decision on lesson organization:
- Repo 1: 
    - modified from https://github.com/datacarpentry/r-spatial-data-management-intro/
    - Episode 1: Spatial data formats
        - file types
            - vector file types, what is a shapefile, what is a geojson object
            - raster file types
            - geospatial databases?
            - geographic and projected coordinate systems - what they are, why they matter, how to select them
    - Episode 2: Project organization and management
        - some from https://github.com/datacarpentry/r-spatial-data-management-intro/blob/master/_episodes_rmd/02-spatial-data-formats.Rmd
    - Episode 3: Spatial data landscape

- Repo 2: Introduction to R for Spatial Data
    - modified from https://github.com/swcarpentry/r-novice-gapminder (episodes 1-6?)

- Repo 3: Raster and Vector Lesson
    - modified from https://github.com/datacarpentry/R-spatial-raster-vector-lesson

Note: Teach data cleaning in the context of the other lessons, not in the first lesson. It is easier to understand once people understand data structures.

2) Docker images
- Deciding whether to use a Docker image for installation. 
- There are dependency issues when working with sf objects. 
- Geospatial packages are complex and have lots of dependencies. Often very challenging for people to install on their own. Takes 
a lot of workshop time and success not guaranteed. 
- Geospatial data are very large. Usually wouldn't work on your laptop. A proper workflow would teach cloud. 
- Precedent in Data Carpentry Genomics lessons for working with pre-installed software (in that case on AWS). 
- With a Docker image, students may not be able to get back into the materials on their own. Harder to use the knowledge they've gained.
- Docker reduces the possible points of failure. 
- Could introduce Docker and at the end of the lesson provide learners with materials for installing software on their own.
- Could have Docker available as a backup for people who aren't able to get the install working. 

Decision:
- Have a couple of the Maintainers test installing all of the software for these lessons on the three major platforms (Mac OS, Linux, Windows) and note any issues. Add these to the setup instructions for the lessons. Set up a Docker image as a backup and also add to the setup instructions. 


4) Topic domains
- Deciding whether to add demographic data to the lesson. 
- This would be part of the canonical two day workshop, not an optional extra lesson. 
- The decision to move from base R plotting to ggplot opens up a lot of time to look at demographic data. 
- Makes the lesson more accessible. 
- Can access the US census bureau API through tidycensus. 
- ggplot2 has census data built in. Has country and state identifiers. 
- This could also be used with interactive mapping. 
- Question about whether it would be a problem for workshops outside of the US to use US census data. 
- Biggest problem is projection - everything is centered in the Americas. Nordic countries need to use projections. 
- Possible open structured exercise where students get data that's interesting to them and subset it to a location that is interesting
to them. A bit ambitious. Natural earth package (rnaturalearth). 

Decision:
- Add demographic data to the lesson in time cleared by moving from base R plotting to ggplot. 
- No specific decision about which demographic data to add.

5) Other notes
- Support was voiced for developing non-R based lessons in the future. Particularly for Python or GDAL (geodata spatial abstraction library). 
- Ideas for other lessons:
    - Leveraging Geocoding and other APIs with OpenRefine
    - GDAL and OGR for Geospatial Data (maybe with Python?)
    - Visualization for Publication (This could be geo, or general)

Action items:
- Erin: compose notes and update repo
- Erin: Email CAC with decisions from conversations and confirm
- Erin: Coordinate with Maintainers about
    - converting static plotting to ggplot
    - writing new content for interactive plotting with leaflet (Leah has an example lesson)
    - testing out installations on Windows, Mac, Linux and coordinating a docker image as a backup
    - pulling out the sections listed above for the intro to geospatial data lesson and creating a new repo
    - creating a copy of the r-novice-gapminder lesson and modifying for geospatial data
