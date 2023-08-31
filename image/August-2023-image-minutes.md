## 2023-08-30 CAC-DC-Image Meeting

* Meeting connection information: [Zoom meeting](https://openmicroscopy-org.zoom.us/j/83692938188?pwd=Yzc4Yk5tOFYxbTVQcHpMODdDSU0yQT09)
* Date and time: [August 30, 2023, 20:00 UTC](https://www.timeanddate.com/worldclock/fixedtime.html?msg=CAC+Meeting+DC+Image+Processing&iso=20230830T20&p1=1440&ah=1)

### Sign-in

* Josh Moore (notes)
* Erick Ratamero
* Ulf Schiller (facilitator)
* Marianne Corvellec (timekeeper)
* Toby Hodges

### Agenda

1. Contributing guide https://github.com/datacarpentry/image-processing/issues/296
    * cf. also Transition to new import convention for sckit-image? https://github.com/datacarpentry/image-processing/issues/295
2. Marianne can share a story following the two Outreachy internships offered by scikit-image to report (qualitatively) on the potential dissemination of the DC Image Processing curriculum.
3. Marianne would have a question (maybe something I missed with the Workbench transition? sorry this might be more maintainer-level than advisor-level): Now development (contribution) at https://github.com/datacarpentry/image-processing happens on `main` (not `gh-pages` anymore), right?
4. Ulf plans to teach DC Image Processing in January 2024, online through Zoom, in collaboration with FZ Juelich/IHRS BioSoft and KIT. Currently planning for up to 300 seats.

### Notes

1. Consensus to use the new full-path style of referencing `skimage` modules.
   Use of `ski` is seen as a step toward general adoption, like `import numpy as np`.
2. Marianne reported on a positive [Outreachy](https://www.outreachy.org/) experience
   which is introducing the curriculum to new communities.
3. Ulf and Toby clarified the branch handling after the transition to the Workbench:
   development is on main.
4. Ulf's teaching of the curriculum on a large-scale (approx. 300 learners)
   is an exciting next step that can hopefully be reproduced elsewhere.
5. Toby added a great first contributor experience recently on the curriculum.
   There's a general agreement that introducing the curriculum to new communities
   has the opportunity to widen it's developer and user reach.

<details>
  <summary>
  Raw notes
  </summary>
  
* Nothing major on the lesson (US)
  - TH: didn't remember opening 296. :smile:
  - MC: issue opened today but didn't have time to look at it.
      - US: histogram in one of the lessons and has shown up differently for someone compared to the one on the website. due to change in imageio/datatypes (e.g., conversion to float)?
  - US: another issue was opened for read-only arrays, but perhaps someone didn't have the latest version
    - https://github.com/datacarpentry/image-processing/issues/285?
    - MC: should be resolved but would like feedback from the submitter
  - MC: any "standard" of how long to leave things open?
    - have something similar for scikit-image. after 6 months a bot can respond
    - TH: within curriculum team have discussed something similar, but not there. no standard exists.
      - in this case, the thing to do is to have a maintainer close it saying as much (tagging the opener)
      
* Contributing guide (US)
  - Good idea, but a question on the import convention
  - Nothing left to do? MC: fine for it to be closed, but important to consider the "generally agreed way" to do it.
  - Background: no longer a technical reason to not import `ski` since lazy loading is now implemented.
  - US: if `ski` is imported that you can automatically access modules? MC: yes. Makes some maintenance tasks easier.
    - US: keep an eye on it.
  - JM: possible educational benefit of using "the normal way"
  - TH: could help to make it "the normal way"
  - MC: scipy was sp, then dropped it, and now they are back. never too late to update it.
  - MC: additional question is how we mention it in the text? `ski.blah`, `skimage.blah`, etc.
  - TH: Worth saying that we are pretty inconsistent on imports in the lesson TBH: https://datacarpentry.org/image-processing/03-skimage-images.html#first-import-the-packages-needed-for-this-episode
  - ER: can try to improve the consistency by using full paths everywhere.
  - TH: do particularly want to avoid import anything from anywhere since you lose the connection. `import numpy as np` was a clear win. Ok with doing that for `ski`, too.
  - US: suggest leave the issue open and we will except pull requests (to adopt the new style)
  - **Generally agreed.**
  - MC: Additional question of talking about the library in text
    - `"scikit-image" or "skimage" or "scikit-image [skimage]"`
    - Also not spelled out on the scikit-image page
    - MC to follow up on this further.
    
* Branch where development happens
  - main vs. gh-pages?
  - **development is on main**
  - gh-pages is generated by GHAs.
  - TH: there is also a legacy/gh-pages branch which is the last state before the transition.
  - US: documented in the workbench
  
* [Outreachy](https://www.outreachy.org/) story (MC)
  - Two projects, suggested both students to work on both projects with both mentors ... (Separated later)
  - Attempted an interesting bioimaging task that can be demonstrated.
  - Strong application period to get-to-know led to strong students.
  - Suggested following the IP curriculum
  - Leading to interest in development e.g. an imaging community in Nigeria :tada:
  - "A way to contribute would be to follow/update/teach the lesson"
  - Opporunities for further dissemination
  - Hopefully spreading like mushrooms :mushroom: 

* Upcoming training (US)
  - Was contacted by future colleagues teaching the curriculum in a massively online 
  - First time teaching it :tada:
  - TH: interested to hear how it goes (need helpers!)
  - JM: open to others? can you share a link?
  - US: no link yet, I think they probably would open it. They were confident in filling it - I will check with the organisers
  - JM: wonder if they are part of an NFDI (nationwide data initiative, I am part of one for Bioimaging NFDI4BIOIMAGE)

* TH: Summer 
  - https://github.com/datacarpentry/image-processing/pull/292
  - Wonderful contribution. Highlight of the working year.
  - Hopefully we will see much more.
  - JM: depending on the motivations, potentially a community that can be accessed.
  
* US: discussion for the future
  - follow-up lessons that we could consider

  </details>