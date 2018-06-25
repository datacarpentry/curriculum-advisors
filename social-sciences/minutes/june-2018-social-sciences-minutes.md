### June 2018 Meeting of the Social Sciences Curriculum Advisors

There were two meetings held:
- Friday, June 15, 2018 at 16:00:00
- Tuesday, June 19, 2018 at 19:00:00

Attending (meeting one):  
- Erin Becker  
- Stephen Childs  
- Peter Smyth  
- Scott Peterson  
- Reka Solymosi  

Attending (meeting two):  
- Erin Becker  
- Geoff LaFlair  
- Peter Smyth  
- Scott Peterson  
- Laura Fortunato  

Detailed Agenda: https://docs.google.com/document/d/1wUDBSzeAoL89ip-PT8yG5zLNDKC1HTHsvYfwnPeNEwg/edit#heading=h.2veemtniyso1 (includes meeting notes)

#### Overall goals
- Decide on action items for resolving any large-scale structural and organizational issues in preparation for publication of the SQL and Python lessons and the R database episode.  
- Evaluate the structure/organization of the published lessons (Spreadsheets, OpenRefine, R) and discuss proposed large modifications.  

##### A1. Structural similarity of Python and R lessons

There are currently significant difference in content between the R 
and Python lessons. There is no need for these two lessons to be 
equivalent, but the CAC should make an explicit decision about 
whether these lessons should be distinct in content and if so which 
differences are appropriate. The table below compares the content in
each of these lessons as of June 6th, 2018. The number is parenthesis
indicates the episode number where that content appears. Areas of 
significant difference are highlighted. 

For each of these areas, the questions are: 
- Is there a compelling reason that learners using one programming language vs another would need to know this particular topic? 
- If no, should it be included in both lessons, or taken out of both lessons?

Individual areas of difference: 
1. Conditionals
    - In R, people are discouraged from using conditionals.  
    - **Decision - Keep in Python, Do not add to R**
2. User-defined functions 
    - **Decision - Do not add to R, No consensus for removing from Python**
3. JSON
    - Very hard to avoid coming across JSON datasets in Social Sciences. 
    - Most people in the room have used JSON formatted data.
    - Often use API calls in R and get JSON formatted data.
    - Don't need to look at the structure of the JSON object, can convert to a dataframe.
    - Materials for teaching JSON in R (https://rcatlord.github.io/GSinR/)
    - **Decision - Keep in Python, Add to R**
4. Merging dataframes
    - Merging dataframes should be in both lessons. Really important set of skills.
    - **Decision - Add to R**
5. Pipes
    - Pipes - not an equivalent in Python. More likely to nest functions or save intermediate variables.
    - **Decision - Don't add to Python**


##### A2. SQL lesson

This lesson needs to be updated to use the SAFI dataset so that it is consistent with the rest of the workshop. It currently uses a database called “SN7577”. To show the advantages and power of using SQL, the data should be split into multiple tables. 

Question 1: How can we split the SAFI data into tables in a way that will demonstrate the power of SQL?

- **Decision - make a "Plots" table which shows the type of crop, number of crobs, size of plot, unit of plot size, etc.**
- **Decision - publish SQL and Python lessons by end of September.**

##### B1. Dataset

The SAFI dataset used in these lessons is real survey data relating to households and agriculture in Tanzania and Mozambique. It includes categorical, numerical, and date data as well as geospatial data (GPS latitude, longitude, and altitude). It also includes data that can be converted to boolean values. The teaching dataset includes data on 131 households in three villages. 

Question 1: Does this dataset represent all of the data types commonly encountered by social scientists? If not, can we incorporate those data types into this lesson without adding an additional dataset? 


Individual items of dicussion:
1. Dataset size
    - There are about 2,000 rows of data available for the SAFI dataset. 
    - People in the room work with datasets from 70 to millions of rows long.
    - An n of 131 is realistic for a master's level student.
    - Learners want to know that the tools they’re being taught won’t break when they use larger datasets. 
    - **Decision: Include more rows in the lesson if possible, but not critical.**
2. Ordinal variables
    - Most people in the room work with ordinal data.
    - Can do this with either posessions (cheap, medium value, expensive) or house types (mud, brick). Both of these have an implied order.
    - **Decision: Add ordinal data using one of suggestions above.**
3. Free text responses, sentiment analysis, other qualitative analysis methods
    - Would be really hard to do this in the time allowed. 
    - Something people would be interested in, but doesn't fit into this workshop.
    - **Decision: Don't add to this lesson. Continue discussions about this for other workshops (e.g. Digital Humanities).**

##### B2. Additions to specific lessons

The Spreadsheet, OpenRefine, and R lessons are currently very similar to the corresponding lessons for the Ecology workshop, however, the needs of these two communities are different and there may be specific changes we should make to the lessons to accommodate these differences. 

Question 1: What metadata standards exist for social sciences? The Spreadsheets lesson includes a section on metadata, but doesn’t currently point towards accepted community standards for metadata for the social sciences. What resources should we incorporate into this part of the lesson?

Discussion:
- Golden standard doesn’t exist right now. Many different domains included with different data types.
- Lots of different groups putting together standards in different areas. May be best to include pointers to different proposed standards in different domains. 
- Some resources:
    - https://www.ddialliance.org/
    - https://ota.ox.ac.uk/documents/creating/dlc/chapter3.htm
    - http://linguistics.berkeley.edu/~jcgood/bifocal/GentleMetadata.html
    - http://www.rnld.org/metadata 
    - https://www.ukdataservice.ac.uk/deposit-data/preparing-data/documentation 
- **Decision: Collect a set of resources to link to.**

Question 2: Should we include a section on historical dates? The Spreadsheets lesson includes an episode for working with dates and includes a short note about problems working with historical data (pre-1899) in Excel. Do social scientists commonly work with data including dates before this time? If so, how can we incorporate this into the lesson?

Discussion: 
- Many people work with pre-1900 data. 
- Breaking it out into year, month, day solves the problem. 
- **Decision: Move this out of the callout to main text. Explicitly mention that breaking into year, month, day solves this problem.**

Question 3: Are there other OpenRefine capabilities we should cover? There are many capabilities that OpenRefine has that we don’t discuss in our lesson. Which (if any) should we add to this lesson?

Discussion:
- The Library OpenRefine uses a lot of GREL expressions, reformatting dates, reformatting names. People say that’s where they tend to spend a lot of their time.
- LC lessons also include data reconciliation. 
- Add something to talk about packages/extensions and their power.
- **Decision: Use LC lesson as source for expanding this lesson, especially in the above noted ways.**

Action items:
- Erin: compose notes and update repo
- Erin: Email CAC with decisions from conversations and confirm
- Erin: Coordinate with Maintainers about
    - Adding JSON to the R lesson
    - Adding merging dataframes to the R lesson
    - Making a "Plots" table for the SQL lesson
    - Publishing the SQL and Python lessons by the end of September
    - Getting more rows of the SAFI data to use in the lessons
    - Adding section about ordinal data to both R and Pythong
    - Adding list of metadata resources to Spreadsheets lesson
    - Moving discussion of historical data to main text of Spreasheets lesson
    - Incorporating data reconciliation, packages, and more GREL into the OpenRefine lesson
