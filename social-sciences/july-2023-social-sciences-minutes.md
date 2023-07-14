**July 2023 Meeting of the Social Sciences Curriculum Advisors**
**Date:** Friday 7, 2023 at 16hs (GTM-3)

**Attending:** Nathaniel Porter, Claudia Engel, Daniel Woulfin, Julieta Arancio, Macarena Quiroga, Erin Becker (Guest)

**Topics discussed:**
- Check-in and feedback on communication/collaboration model
    - Generally good start, rough around the edges
    - How to collaborate when not familiar with tools
        - Focus on big picture/curriculum implications (CAC not usually responsible for technical details)
        - Good reminder to try and avoid being too techy

- Curriculum Specific Instructor Onboarding (guest: Erin Becker)
    - Overview
    - Resources / Links
        - [Lesson specific onboarding slide deck template](https://docs.google.com/presentation/d/1VTBWHL5BHPfZ0Ejiuwk5lUGFUGaLTujTs_OfybrEZrA/edit?pli=1)
        - [Library Carpentry Curriculum Onboarding 2023 - as example](https://docs.google.com/presentation/d/1GCqeFDGeiMn3oDTsTOgdspRXqtnKt-WtXyeH_u0pIV8/edit#slide=id.g1b7201a36df_0_103)
        - [Existing onboarding video on YouTube (4 years old)](https://www.youtube.com/watch?v=u4nDomxRVoI&list=PLXLapl_LKb4e73Vf2e3rS2q2TDJ7oh_DX&index=3&pp=iAQB)
    - Discussion
        - Seems helpful, but maybe long?
        - Perhaps offering both video and annotated slides as options, allowing different approaches to learning as well as including optional material that most people may not need in the full slide deck
        - How does this tie into instructor material online?
            - Potential to include in instructor view/notes
    - Is anyone from CAC willing to be a point person for work on this?
        - timeline: no pressing deadline, grant end 2024, progress report by the end 2023
        - goal: onboarding video for this group by the end of 2023 latest; first working on the slides and then the video
        - **Volunteers: Macarena Quiroga and Claudia Engel (help develop), Nathaniel Porter and Julieta Arancio (feedback only)**


- Flagged Issues/PRs
    - Ongoing (or resolved pending PR/Merge)
        - R
            - Merging Dataframes (part of [issue #80](https://github.com/datacarpentry/r-socialsci/issues/80))
                - Slack consensus (added to Git) is to make an optional lesson using `join` rather than `merge`
                - **Issue now closed**
            - [Cleaner SAFI_clean dataset](https://github.com/datacarpentry/r-socialsci/issues/446)
                - There are various discussion items around this dataset and how easy is to use it for the lesson goals (like pivot_wider/longer, see below, and visualization)
            - [Quarto vs. RMarkdown](https://github.com/datacarpentry/r-socialsci/issues/459)
                - Action (per slack) stick with Markdown and revisit later 
                - **Issue now closed**
        - OpenRefine
            - [Messier Data](https://github.com/datacarpentry/openrefine-socialsci/issues/108)
                - **Slack consensus (added to Git) is to encourage implementation and recommend mentioning character encoding**
    - New
        - R
            - [Changes to R handout](https://github.com/datacarpentry/r-socialsci/pull/466)
                - What's the benefit compared to tidyverse cheatsheets and how do people use them?
                - Also how will these be maintained to keep up with lesson changes?
                - **onepage is better for searching (and using limited scope)**
        - OpenRefine
            - [Getting Help/Other Resources Section](https://github.com/datacarpentry/openrefine-socialsci/issues/122)
                - **Important to have the extra help somewhere and in one place (exactly where matters less) because hard to find openrefine help (including GREL) +1**
                - **Having final episode good, maybe with instructor note to point these out because hard to find help**
        - Spreadsheets
            - [Adding Google Sheets option](https://github.com/datacarpentry/spreadsheets-socialsci/issues/97)
                - **Some people/universities not allowed to work with Google products (for example German universities); may need to have some kind of a warning about privacy/ethical issues**
                - Also widely used and helpful
                - Use depends on data - esp GDPR/PII/etc
                - **Probably need to have some kind of disclaimer if included (always be careful with data, who has it, etc and check with your institution/etc)**
                    - If it's in a Carpentries lesson, can it be seen as an endorsement?
        - Social Science Workshop
            - [Changing from SAFI data](https://github.com/datacarpentry/socialsci-workshop/issues/49https://)
                - This would be good opportunity to think about dataset in concordance with specific neeeds of lessons (without having to do extra complications to exercises)
                - Also somewhat uncomfortable with content (African houses as mudhouses etc)
                - **To be mentioned in issue, see below**
    - Potential
        - improve tidyr lesson in R to make more intuitive/usable
            - perhaps also make tidyr optional (more advanced) although it's very useful and worth knowing about
            - **Macarena will raise an issue about this**

- Future meeting(s)
    - Continue every 2-3 months
    - Next meeting chair (tentative) Eirini Zormpa
