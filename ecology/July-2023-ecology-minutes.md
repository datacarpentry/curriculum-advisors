# July 2023 Meeting of the Ecology Curriculum Advisors  

Meeting took place on **Thursday 6 July 2023 ⋅ 13:00 – 14:00 UTC**


## Attendants

- Mike Trizna, he/him/his, Smithsonian Institution 
- Reinder Radersma, he/him, Netherlands Foundation of Scientific Research Institutes
- Jen Thomas, she/her
- Sichong Peng, he/him, EclipseBio
- Erin Becker she/her, The Carpentries
- Toby Hodges (he/him), The Carpentries
- Adriana De Palma (she/her), Natural History Museum

## Roles

- **Timekeeper:** Reinder
- **Facilitator:** Jen
- **Note Taker:** Toby

## Agenda
- Previous meeting notes (below, and posted to https://github.com/datacarpentry/curriculum-advisors/blob/main/ecology/April-2023-ecology-minutes.md)
- New R Ecology Lesson:
  - Blog post draft: https://codimd.carpentries.org/bofHxJ3wR22WSfhLPDaCYg?view
  - Jen's issue: https://github.com/carpentries-incubator/R-ecology-lesson-alternative/issues/3
  - Toby's comment: https://github.com/datacarpentry/python-ecology-lesson/issues/259

## Previous meeting notes
- Mike: I am putting in a PR to adjust the title but otherwise all looks good (wrong date in title).

## New R Ecology Lesson
### Blog post draft: https://codimd.carpentries.org/bofHxJ3wR22WSfhLPDaCYg?view
- Is the committee happy to go ahead with publishing this?
- Any changes you want to make?
  - Sichong: a few typos but otherwise it's good.
  - Adriana: seems to be missing some formatting e.g. bullet points to help readability
- Mike: regarding lesson repo - only James has agreed to maintain it?
  - Yes, so far. Michael C-M is also following progress. If this lesson does get formally adopted, we would need to ask the other Maintainers if they are happy to switch over to maintaining this one - if not, we can factor that into planning for next Maintainer Onboarding cycle.
- ACTIONS:
  - CAC members review and make changes to the CodiMD source (or send to Toby if you prefer) by end of this week.
  - Toby to prepare a pull request to publish the post to The Carpentries blog
  - CAC members, Curriculum Team to promote this call for pilot workshops on local and global channels:
    - ROpenSci Slack (Toby will ask someone from Core Team to do this)
    - general on Carpentries Slack (Done automatically when blog post is published)
    - dc-ecology-r on Carpentries Slack (Toby)
    - discuss maiiling list (Toby)
    - Toby will also coordinate with members of Workshop Administration Team to let Instructors know they can use this lesson if teaching a DC Ecology R workshop any time soon.

### Jen's issue: https://github.com/carpentries-incubator/R-ecology-lesson-alternative/issues/3
- If CAC does not push for database content in programming lessons, we are losing a key strength of the curriculum. Databases can make life much easier as an ecologist. 
- Adriana: when we ask for feedback on the new lesson version, can we specifically ask if they missed the database section?
- Jen: only concern is that people won't know what they were missing.
- Sichong: agree it would be helpful to include info about how to work with databses in R or Python. Based on my experienc eteaching workshops, these parts get skipped often - mostly due to lack of time. SQL is a relatively heavy topic, needs time to develop understanding.
- Toby: does anyone know if the current version of SQL episode could be transplanted as-is? If so, and if CAC feels it's important to include these skills, we could add that episode back in fairly quickly.
- Mike: Otherwise, the Incubator could be a good place for this content, so that it doesn't get lost altogether. The episode definitely relies on whether Instructors have also taught the SQL lesson.
- Reinder: we use relational databases a lot but not SQL very often. A lot of alternatives popping up, no clear one to go for instead. I wonder if anyone else has the same feeling?
- Jen: perhaps we should be thinking about relational databases and SQL as two different aspects?
- Reinder: in that sense might also be worth thinking about whether you want to teach people SQL, or only to raise awareness that people can do this kind of thing.
- Adriana: beta courses feels like an intro to ecology - relational databases seems like an intermediate step. Most beginner students will only use relational databases after it has been pre-filtered and downloaded as a standard csv file. If you want more idetail in the course and to move it into a more intermediate stage, then I'd agree that having a broader approach to relational databases rather than focussing on the detial of sql would be more useful. I like the idea of a lesson that pulls and combines data from different sources and database styles - this feels more and more relevant as ecology expands into what was traditionally data science territory.
- Next steps? What are our options?
  - Do not include it in R-ecology-lesson-alternative, and ask about whether it is missed?
    - Adriana: and add to the blog post, mentioning that it is not included and asking anyone who wants it to be there to 1) tell us, and 2) write it.
    - Adriana: I vote for this option, as it would feel really tacked onto the end of the lesson.
    - Mike too
  - Or include it, and ask about whether people taught it and how it went?
    - Sichong: I vote for this, to include it until we gather more feedback.
  - ACTION: Toby will adjust blog post to invite feedback on the DB content being excluded. He will also adjust the feedback issue form to ask about whether it was missed by Instructors, learners.

### Toby's comment: https://github.com/datacarpentry/python-ecology-lesson/issues/259
- Jen: relevant to previous discussions about whether Python and R lessons should follow a similar structure
- Mike: I could create a rendered version with the proposed changes
- Toby: you will need to adjust Katrin's Markdown to work with the new lesson infrastructure.
- Mike: we could respond that this is not feasible.
- Toby: could be argued that you would be better off waiting for feedback on redesigned R lesson
- Adriana: what they have described certainly makes sense. Although if we're moving to the beta R lesson version, then matching up Python will be more work than only these changes.
- ACTION: Mike will respond to issue, pointing to blog post and saying that we will wait for feedback on that.

**Next Meeting: September 18**
