# July 2022 Meeting of the Astronomy Curriculum Advisors  

Date: July 18, 2022, 21.00-22.00 CET 
 
## Attendants

* Azalee Bostroem
* Heather Andrews
* Ivelina Momcheva
* Phil Rosenfield
* Adam Hughes
* Rachel Lee McClure
* Meredith Rawls
* Erin Becker

## Roles

**Facilitator:** Azalee

**Notetaker:** Meredith

**Timekeeper:** Heather

## Agenda

### New lesson maintainers 

* There are **two new lesson maintainers**: David DeMuth and Ralf Kotulla

* **Shall we meet with the maintainers?** That is left to our discretion. Maybe we can invite them to a future meeting.

### How do we keep lessons up-to-date with changing software? 

* There have been some issues and lesson-breaking situations due to changes/updates in some software used in the lesson. The issues range from e.g. numpy warnings (unintentionally teaching to ignore warnings...) to errors that required modified the lesson substantially (e.g. Gaia updated ADQL so the polygon function can only run on coordinates and not on proper motions as taught in the lesson).

    - (Phil) Dealing with changing software can also be used as a **teaching moment**.  
    - (Iva) Is there any kind of **automated testing** on lessons? That could flag the issues, and then maintainers could be assigned/requested to fix the issues.  
        - The problem is that most issues have not been solved by the time a workshop takes place.  
        - (Erin) Carpentries does have some infrastructure options for integrated testing.  
        - (Meredith) This kind of problem is very common in Rubin. We could add a requirements.txt with explicit python library versions (akin to what Rubin does).  
        - (Rachel) We can leverage the conda environment we ask the learners to set up.  
        - (Heather) There is a yml file along these lines, but the only thing presently specified is python>=3.6. In any case the question remains for when/how we should update this.  
    - (Azalee) Is doing this versioning/dependency updates a reasonable expectation for maintainers?  
        - (Erin) Yes, as long as we are talking about minor versions (not e.g. python2 to python3)  
        - (Phil) We should keep a realistic estimate on how often this kind of update work is needed and how long it actually takes; if it's 1-2 times a year that is probably feasible.  

* Unofficial vote on whether we think **keeping a versioned list of pinned packages** makes sense and put it in the yml file.   
    - Everyone voted **yes**  

### AAS report 

* Azalee and Adam were in this workshop. This is the **first in-person workshop** with this curriculum. 

* Things **did not go faster in person than on Zoom**.  
    - May need to cut some of the curriculum.  

* Participants **did not follow the setup instructions**.  

* Few participants did not come back for the second day.  

* Big issue: the **Gaia database was down** during the workshop due to Data Release 3 prep. Azalee spent a lot of time on a last-minute workaround, which added a layer of complexity to the curriculum.  
    - (Heather) Are there any plans for sharing the workaround?   
        - (Azalee) We could have a warning on the instructor prep/guide page and suggest instructors to reach out to us if a workaround is needed.   
    - (Iva) Gaia does not have that many more data releases planned.  

* The plan now is to **submit for winter AAS**. Deadline is Aug 2, 2022.  

* Pre/post **surveys** and post-it **feedback**:  
    - General appreciation of helpers and content.  
    - Some (especially undergrad) participants expressed that pre-requisites were not sufficiently clearly laid out.   
    - Some participants prefer the modality of "give me the notebook and let me click through".  
        - It could be evaluated the option of having a **printout** available, since the lesson currently involves a lot of typing.  

### History of Curriculum

* Azalee gave a brief presentation about the history of the astronomy curriculum. It began as an idea in 2017 spearheaded by Azalee and Rudy. Allen was hired as the lesson writer. AAS members were queried about what should be covered (e.g., file formats, tools, workflows). 
    - (Phil) (How) Should we send a **feedback survey** out again to registered participants? (or more broadly to the astronomical community)     
        - (Erin) We would need a concrete plan for using the results of the survey.  
        - (Phil) It would be interesting to see if we are on track and how to inform the next thing we should develop.

* (Iva) It has happened that learners expect to learn/use **scikitlearn or maching learning** techniques. Perhaps of interest for future lessons/curricula? https://archive.stsci.edu/hello-universe 
    - (Azalee) Not sure about future of the field converging on some "universal skill set" and whether machine learning is on that list. Question to think about: *is there something we could take out of the current content and put machine learning in its place? do we need a new curriculum?*
    - Possibility of **asking participants** directly about what would they add to the current contents.
    - (Phil) Knowing whether the community has an unmet need for a machine learning lesson is worth asking, but might be more useful in a "bring your own data" kind of workshop.  

### (Continuation from last meeting) Goal could be to continue to look out for gaps in astro education that we can fill, whether that means funding for another curriculum developer or drafting mini lessons, etc. 

* (Azalee) We need to be thoughtful about how many versions/lessons/curricula we can realistically maintain at a Carpentries level. Software Carpentry taught to astronomers often condenses the shell lesson (because most astronomers have at least some exposure already), so there's ~half a day to fill with other content: **what similar flexibility might we have in this curriculum?** Or should we just leave it as-is for now? Perhaps wait for Rubin/JWST to change the landscape a bit?  
    - (Rachel) Have **modules** for different science questions and different primary tools.  
    - (Azalee) The curriculum is currently extremely cumulative and not modular at all.  
    - (Meredith) We need the existing curriculum "story" to get everyone on the same page with common astro tools. The next level could be **dataset or science specific**. But maybe that's too many levels since CAC needs to come after the Software Carpentry.
    - (Azalee) Perhaps add link to external resources as next steps instead?
    - (Phil) There are plenty of use cases and problems that need solving. Who is our audience?
        - (Iva) Carried out surveys in the past on **what tools astronomers would like** (perhaps summarize those results for next meeting). Could ask Gaia researchers what directions dataset could most easily go for learning certain methods.
    - (Adam) Focus on **carpentries methodology of layers** building on top of each other.

### Gaia DR3 update (to be discussed in the next meeting)

## Wrap-up

* Questions to think about:
    - What questions should we be asking our participants or the astronomy community at large?  
    - Who is going to actually do this work?

* Reminder we have a Slack channel for followup chats in the Carpentries Slack, #cac-astro  