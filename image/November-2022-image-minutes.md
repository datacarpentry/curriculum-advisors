## 2022-11-18 CAC-DC-Image Meeting 

* Date and time: [Friday, November 18, 2022, 18:00-19:00 UTC](https://www.timeanddate.com/worldclock/fixedtime.html?msg=CAC+Meeting+DC+Image+Processing&iso=20221118T18&p1=1440)

### Attendents

* Marianne Corvellec (timekeeper volunteer)
* Josh Moore (notetaker volunteer)
* Erick Ratamero
* Ulf Schiller (facilitator volunteer)
* Sunil Shende, arrived late due to DST and was not present for any of the votes (🗳️)

### Meeting roles

* Facilitator - Introduces each agenda item. Monitors both the chat and the visual meeting window for “hands”, keeps track of order, and says whose turn it is to speak. Makes sure everyone has a chance to share their views.
* Notetaker - Records meeting attendance and major points of discussion. Especially takes note of decisions and action items.
* Timekeeper - Pays attention to the clock and notifies the group when time for specific agenda items is running short.

### Agenda

1. Welcome and introductions
    * Ulf: Work over the past year after new maintainers found which helped to move towards the "Beta" stage.
    * Erick: JAX, dededicated team of 4 people on data management & image analysis. Worked on "RMS-Approved" processing while in the UK.
    * Josh: OME developer, focused on research data management. Beginning NFDI4BIOIMAGE funding to connect research data across Germany.
    * Marianne: scikit-image core developer, funded for OSS. EOSS funding as main contract. (Also on the literary side). Focused on the dissemination side of things. Physicist by training.
    * Ulf: material scientist at Clemson (but also computer science and physics). Liquid materials, HPC. Reconstruct images in 3D. Use many of the carpentries for students.
3. Meeting logistics (document sharing, note taking, etc.)
    * All ok with codimd? 🗳️ **Vote**: 4 yeses.
    * Josh to open a PR with the notes (Ulf to review and approve)
    * General preference for setting meeting times for the entirety of our term
    * Re-iterating the encouragement to use "raise hand" or type "hand" (if you can't find a way to break into the conversation)
4. Discussion of voting procedures
    * Q: Define quorum?
      * Ulf: "Not more than one person missing"? All agreed.
    * Q: Require unaminity or majority vote?
      * Marianne: prefer "common-sense unaminity". Ulf: we'll formulate that as the goal for all votes, "striving for". All agreed.
    * Can be revisited.
5. Discussion on `skimage.io` and `imageio.v3` (see Github issue [#239](https://github.com/datacarpentry/image-processing/issues/239))
    * Josh & Erick reviewed the issues/PRs beforehand.
    * Marianne: encourage people to use the realistic libraries now. (imageio supports metadata. good vision & practices.)
    * Josh: (Playing devil's advocate) Does the conversations about the _next_ lesson help? i.e. could we end with "there are other libraries?"
    * Ulf: Perhaps helps to reduce "cognitive load", but there's a compromise to make. but useful to teach the way it will be done.
    * Erick: Conceptually agree with "just use imageio", i.e. it makes sense to decouple IO and the processing (with numpy in the middle)
      - If we're extending to the cloud, then you replace with dask/zarr but you're still getting a numpy array.
      - Also, just replacing skimage.io with imageio doesn't increase the cognitive load.
    * Ulf: and the work is already done :smile:
    * Marianne: `as_gray` keyword is intuitive, whereas `mode="L"` is not: not all updates are perfectly satisfying (burden is more on the teaching side).
    * Ulf: also assume that Toby is happy with the change.
    * Marianne: good timing as we move towards "Stable".
    * Josh: can see thematicizing "loading a numpy array" as a section. Agreed. Josh to open an **issue** 📝
    * 🗳️ **Vote**: 4 yeses
6. Discuss (and potentially vote) on approving the Data Carpentry Image Processing with Python curriculum to be moved from “beta” to “stable” status.
    * Toby's video: https://carpentries.zoom.us/rec/share/asqmFpStsNf-hLZpLrsXCDkjBRQds-LnhSqaIlVS4WPEkK1HuDdXMluzC3q1nZ6p.FXhezAk8bdHjJmNI (Passcode: a6=eUJye)
    * Ulf: didn't get 100s of bugs when moved to "Beta"
    * Notable feedback/suggestions from pilot workshops
        * lesson ends somewhat open ended/conclusion unsatisfactory
        * selection of images somewhat incoherent and not closely related to "scientific" images
          - One open issue suggests using _fewer different_ images. Decided against.
    * Ulf: Don't particularly feel that they are blockers especially considering the demand.
    * Josh: what would constitute a "breaking change"? (What form of semver, etc. applies?)
      * Erick: essentially there's no "breaking change". The material is just the current version.
    * Erick: no content issues, nor with the images.
      * Would like there to have "light" and "dark" backgrounds for segmentation and thresholding.
      * Marianne: a bit unfortunate that all the images have the same dtype. Maybe the arbitrary change to `(0, 1)` is _sufficient_ to expose learners to other formats?
      * Ulf: good point. Again worth an **issue**. 📝
    * Marianne: important to provide the right conceptual boxes, but even that can be changed (for new students)
    * Ulf: there could be of course be updates, but that's natural.
    * 🗳️ **Vote**: 4 yeses
7. Plan next meeting
    * "Edge detection" bonus episode (see Github issue [#241](https://github.com/datacarpentry/image-processing/issues/241))
      - Ulf: don't see any damage in keeping in.
      - Marianne: propose to table. (As timekeeper...)
      - Done: 18:58 UTC
8. Any other business
    * Marianne (for Toby _et al._): Can we see the rendered lesson for a given PR? CI seems in place but jobs were skipped...
    * Sunil: joins unfortunately with an off-by-one timezone error
      - Name "Channel" is introduced without any explanation.
      - Ulf: good point. That would be a good **issue** 📝 to open in the repository (if it does not exist)
