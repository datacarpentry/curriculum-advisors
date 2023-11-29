## 2023-11-29 CAC-DC-Image Meeting

* Meeting connection information: [Zoom meeting](https://openmicroscopy-org.zoom.us/j/83692938188?pwd=Yzc4Yk5tOFYxbTVQcHpMODdDSU0yQT09)
* Date and time: [November 29, 2023, 20:00 UTC](https://www.timeanddate.com/worldclock/fixedtime.html?msg=CAC+Meeting+DC+Image+Processing&iso=20231129T20&p1=1440&ah=1)

### Sign-in

* Erick Ratamero (Timekeeper)
* Marianne Corvellec
* Ulf Schiller (Facilitator)
* Toby Hodges (Notetaker)

### Agenda

* Decide on creating a separate section about image loading: https://github.com/datacarpentry/image-processing/issues/242
* Discuss linking to checklists for publishing images and image analyses: https://github.com/datacarpentry/image-processing/issues/303
* Future plans for Curriculum Advisory Committees (optional, whatever time we have remaining)
* Develop parallel curricula with different (real-world) example datasets?

### Notes

* Decide on creating a separate section about image loading: https://github.com/datacarpentry/image-processing/issues/242
    * Marianne: think we should make a decision; willing to start a PR if needed
    * Ulf: I don't think there has been a lot of dissent
    * Erick: I like the idea for the curriculum
    * Ulf: I will teach some of the material in January, probably have extra time to spend and have been asked to do some more general stuff that is not specific to Python. Will think about how to integrate stuff about image capture workflow/pipeline and could contribute.
    * Erick: I will also be teaching this more next year.
    * ACTION: Marianne to draft a pull request to add this section; Ulf to contribute based on experience teaching related content in January.

* Discuss linking to checklists for publishing images and image analyses: https://github.com/datacarpentry/image-processing/issues/303
    * checklists from [_Quarep-LiMi_](https://quarep.org/), a project promoting quality assurance and reproducibility in light microscopy.
    * seem very relevant to our target audience.
    * question is where to put these/refer to them in the lesson?
    * (not directly relevant: that working group is now looking at developing teaching materials to promote some of the practices they recommend - potential for complementarity with our curriculum)
    * Erick: another relevant and similar effort is REMBI: https://www.nature.com/articles/s41592-021-01166-8
    * Erick: there is another paper that would be relevant, ~~if I can dig it up~~ https://www.nature.com/articles/s41592-023-01919-7, providing a flowchart etc to help you make decisions about tools and analyses to perform etc depending on your data and other things
    * Ulf: I like the idea of a group coordinating the development of these kinds of materials, avoid de-duplication of effort.
    * Erick: perhaps we can compile a list of useful resources, not all of which need to go into the curriculum
        * Toby: these could be added to https://github.com/datacarpentry/image-processing/issues/144
        * Erick: I think these resources will be slightly different from what has been collected in that issue so far.
    * Toby: I am happy to open a PR for this, but would like guidance about where
    * Ulf: I can scope this out in January
    * Erick: I think this makes sense in the very last episode, suggested further reading
    * Toby: might need to re-title the final episode
    * Marianne: or add a new episode in its own right?
    * Ulf: I like that idea, because this could get quite substantial. @Erick please add what you have to that issue, and I will try to convert into a new episode.
    * Ulf: I will also reply to the issue to give other maintainers a heads-up that things are going to be coming in and that we have a plan to do something with them
    * Erick: the resources may be heavily focused on light microscopy
    * Ulf: we can use that first and try to attract more from elsewhere
    * ACTIONS:
        * Erick to add his list of known relevant resources to issue #144
        * Ulf to reply to #144 to give Maintainers a heads up about the incoming resources and what is going to be done with them
        * Ulf to convert Erick's list of resources into a new episode, called _Further Reading_ or something similar
        * Committee members to add to that list/encourage others in their networks to do the same

* Develop parallel curriculum with different (real-world) example datasets?
    * On the Quarep call earlier, Christian Tischer again raised the idea of developing a parallel curriculum with alternative example data. Toby suggested he speak to Curriculum Advisors about this. So Tischi might join the next CAC call...
    * Erick: We might teach from a fork with different data next year too. Could tie in nicely
