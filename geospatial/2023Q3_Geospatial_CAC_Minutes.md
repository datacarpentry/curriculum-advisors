# Minutes
Data Carpentry Geospatial Curriculum Advisory Committee Meeting
September 20th, 2023 (10am CDT, 11am EDT, 5pm CEST)

## Attendees

- Stephen Appel
- Jeff Hollister
- Mike Mahoney
- Toby Hodges (Curriculum core team)
- Paula Martinez Lavanchy (Guest)
- Claudiu Forgaci (Guest)

## 1. Introductions and Code of Conduct

## 2. Previous Minutes:

    November 29, 2022: https://github.com/datacarpentry/curriculum-advisors/blob/main/geospatial/2022Q4_Geospatial_CAC_Minutes.md

    March 30, 2022: https://github.com/datacarpentry/curriculum-advisors/blob/main/geospatial/2022Q1_Geospatial_CAC_Minutes.md

## New Business:

### 1. Data Carpentry for Geospatial data for targeting researchers in the Urbanism field (See also, Appendix)

    * https://github.com/Rbanism/geospatial-data-carpentry-tud-2022-11

    * https://github.com/Rbanism/geospatial-data-carpentry-tud-2023-06

    - 2 pilot workshops have already happened

    - submit to the incubator 

    - Workshop Structure

    - Day 1 P1 adapted from Social Science/Humanities workshop

    - Introduction to R

    - Switched Raster and Vector so that V comes first

    - Dropped episodes 11, 12

    - Worked with Open Street Map data which is used extensively in urb. field

    - Built in such a way that localization is possible

    - Summary of changes made:

    - Issue on the incubator URL: https://github.com/carpentries-incubator/proposals/issues/174

    - Replaced the data with data more relevant to urbanists

    - Jeff in favor of pushing along 

    - Mike has questions for Toby

    - Geospatial currently has 3 core lessons

    - Would not be "in addition" to current lessons, would be an alterantive

    - Toby compares to Genomics curriculum and discussions around what will be inlcuded for workshop to be "official" genomics curriculum

    - Different focus, but is still Geospatial

    - Would need approval from data carpentry governance 

    - Skills broadly the same, but different example data/target audience

    -up to the committee if we are satisified that the skillset targets are the same

    - Refer to recent blog post from Ecology: https://carpentries.org/blog/2023/07/r-ecology-alt-beta/

    - In addition to the incubator, there is also the carpentries lab https://carpentries-lab.org/

    -Mike asks if incubator and lab are separate tracks?

    -Toby clarifies that it should be on the incubator and then on the lab

    - Claudiu sees the review process as an opportunity for direct feedback or a more formal (like open sci) approach like the carpentries lab.

    - Editor checklist for the Lab: https://github.com/carpentries-lab/reviews/blob/main/docs/editor_guide.md

    - Reviewer checklist for the Lab: https://github.com/carpentries-lab/reviews/blob/main/docs/reviewer_guide.md#reviewer-checklist

    - info about collaboration with the Journal of Open Source Education: https://github.com/carpentries-lab/reviews/blob/main/docs/author_guide.md#jose-submission

    - In the process of making revisions from second pilot and are confident in the way it works

    - Workshops not planned until after the end of the year

    - Toby will respond to incubator issue ASAP

    -prioritize a call similar to the ecology r lesson 

    - Toby will ask a CAC member to be a sort of editor for the lab review process

    - CAC will decide when to invite for review in the lab

## Old Business:

### 1. Python Fork of Lessons

   - Check back in with Ryan before next CAC meeting

   - Consistent process with proposed urbanism lesson

### 3. Issues: (added to agenda by Mike)

    * https://github.com/datacarpentry/r-intro-geospatial/issues/123

      - because getwd is part of the standard pacakage and additional packages can cause complications and add additional complexity.
  
      - General concensus that it's too much of a distraction
  
      - We recommend an instructor note to emphasize how essential it is that people are in the correct location since everything will be relative paths after (Mike taking action item)

    * https://github.com/datacarpentry/r-intro-geospatial/issues/119

      - Need to update since in R4.0.0+ read.csv has stringsAsFactors=FALSE by default.
  
      - There's a few places in the lessons where this is an issue
  
      - Mike willing to spearhead a modernization project 
  
      - Will bring back any curriculum level questions to the committee
  
      - Toby will respond to issue and suggest Alber closes issue and opens a new issue specifically about the dataset because a sufficient amount of the original issue has been addressed.
  
      - https://github.com/datacarpentry/r-raster-vector-geospatial/issues/368#issuecomment-1501300940


### 4. deprecation of the sp, rgeos, and rgdal packages
     
     - Thanks to the community! 

## Updates:

### 1. Carpentries Workbench

## Appendix:

### Paula's E-mail:

Dear Curriculum Advisory Committee Geospatial data,
 
My name is Paula Martinez Lavanchy and I am the Carpentries membership coordinator at TU Delft and 4TU.ResearchData, in the Netherlands.
 
At TU Delft, we have a community of very enthusiastic certified instructors, who are always happy to contribute not only by teaching, but also thinking on how to bring the Carpentries lessons to their communities of practice. One example, is my dear colleague Claudiu Forgaci (in CC), an Assistant Professor of Urban Design at TU Delft, who together with other colleagues from his department have edited and adapted a bit the curriculum of the Data Carpentry for Geospatial data for targeting researchers in the Urbanism field.
 
They have piloted this adaptation as a mix and match self-organised workshop twice:
In November 2022: https://github.com/Rbanism/geospatial-data-carpentry-tud-2022-11 and,
In June 2023: https://github.com/Rbanism/geospatial-data-carpentry-tud-2023-06 
 
Claudiu and his colleagues are ready to give it a try to convert these pilot into an adapted curriculum for Geospatial data in Urbanism.
 
Toby Hodges, also in CC, has suggested to pitch this idea to the CAC to know if the effort of formalizing the lessons would be welcome. In the meantime, Claudiu and his colleagues will create an issue in the carpentries-incubator for documentation purposes.
 
We would appreciate very much if you could discuss this ideas and provide us with feedback.
 
Thank you very much in advance for your time and response.
 
Best wishes,
Paula
 
Paula Martinez Lavanchy, PhD
