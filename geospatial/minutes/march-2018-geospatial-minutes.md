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

Detailed Agenda: https://docs.google.com/document/d/1VG34gKSzQZg-wrvAuDSp-ExCnVZamc6AcAvfzTsemUc
    
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
- No decision. Dependent on target audience. 

3) Learner level
- Currently lessons don't include any introduction to R. Instructors have been teaching ad hoc introductions to R. Some audiences need the
background and some don't. 
- Don't want to spend too long on intro but can add an introductory lesson to avoid the need to ad lib and make it easier for instructors
to teach the lessons. 
- Can skip the introduction to R if learners have programming experience. 
- Can use the introduction to R lessons from the r-gapminder-novice lessons for SWC. Can tie these data into geospatial and get a 
global perspective. 

Decision:
- Use the r-novice-gapminder lessons as a basis for creating an introduction to R for geospatial. 
- Copy over these lessons and start modification. 

2) Docker images
- Deciding whether to use a Docker image for installation. 
- There are dependency issues when working with sf objects. 
- Geospatial packages are complex and have lots of dependencies. Often very challenging for people to install on their own. Takes 
a lot of workshop time and success not guaranteed. 
- Geospatial data are very large. Usually wouldn't work on your laptop. A proper workflow would teach cloud. 
- Precedent in Data Carpentry Genomics lessons for working with pre-installed software (in that case on AWS). 
- With a Docker image, students may not be able to get back into the materials on their own. Harder to use the knowledge they've gained.
- Could introduce Docker and at the end of the lesson provide learners with materials for installing software on their own.
- Could have Docker available as a backup for people who aren't able to get the install working. 

Decision:
- No decision, but leaning towards providing something as a backup for people who have installation issues. Either AWS or Docker image. 


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
