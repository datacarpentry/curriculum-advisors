# Agenda and Minutes for December 10, 2025 Genomics Curriculum Committee Meeting

4 pm CST (GMT-6) via Zoom

Attending: Naupaka Zimmerman (@naupaka), Sehrish Kanwal (@skanwal)

- [X] **Action Item:** Naupaka to open PR with these minutes to the following repo and and Sehrish will comment/approve/merge.
    - https://github.com/datacarpentry/curriculum-advisors

## Moving R-genomics out of beta

It is time to consider moving the R-genomics lesson out of beta status into active status. [This is the SOP on promoting a lesson to active status from beta](https://docs.carpentries.org/handbooks/curriculum_advisors.html#issues-for-which-maintainers-must-seek-cac-approval). It requires the curriculum committee to review the lesson and vote on whether to promote it.

The lesson has been in alpha/beta since its creation. In May 2022, it was formally taught during a beta pilot, which resulted in a [set of notes and issues to resolve/adjust](https://github.com/datacarpentry/genomics-r-intro/issues/142). These have almost all been addressed, and the only two remaining are minor and can be resolved post-promotion.

Upon approval, the maintainers will need to update the lesson status in the lesson repository and also notify the Carpentries website team to update the website.

See [genomics-workshop issue #166](https://github.com/datacarpentry/genomics-workshop/issues/166#issuecomment-3541611640) about updating the overall workshop schedule to indicate R-genomics is out of beta.

Also see merged [datacarpentry.org PR #78](https://github.com/datacarpentry/datacarpentry.org/pull/78#issuecomment-3542118714) about updating the website with the new lesson status.

- [ ] **Action Item:** Sehrish to comment on [this issue](https://github.com/datacarpentry/genomics-workshop/issues/166#issuecomment-3541611640) and [this PR](https://github.com/datacarpentry/datacarpentry.org/pull/78#issuecomment-3542118714).

- [X] **Action item:** Naupaka posted an issue on the [R-genomics repo](https://github.com/datacarpentry/genomics-r-intro/issues/325) to notify the maintainers to update the lesson status in the repo.

**Vote:** 2/2 in favor of moving lesson to stable.

## Review shell-genomics PR #371

The idea is to change the grep content to focus on parsing a metadata file instead of a fastq file to lower the cognitive burden and avoid some technical issues with grep compatibility across systems. It also removed the shell arithmetic section which was deemed too advanced for the target audience.

[feat: change grep & redirection exercise to use metadata instead of fastq #371](https://github.com/datacarpentry/shell-genomics/pull/371)

We discussed this PR and agreed it generally seems like a good idea. However, we’d both like to run through the new material step by step to get another set of eyes on the flow and how it might work for a learner. Once we do this, we will comment on the issue and at that point should be considered to have the approval of the committee.

- [ ] **Action Item:** Naupaka and Sehrish to test PR 371 as learners (probably locally just for convenience). The instructions for running the lessons locally [are here](https://datacarpentry.github.io/genomics-workshop/index.html#option-b-using-the-lessons-on-your-local-machine).
- [ ] **Action Item:** After testing, both Sehrish and Naupaka to comment on the PR with their approval.

**Vote:** 2/2 in favor of merging PR, pending testing by both Sehrish and Naupaka first.

## Revamp of DC Cloud Genomics materials

**Context:** In early 2025, Ben Busby and Emily Page (?) reached out to offer to help with an overhaul and modernization of the [cloud genomics DC lesson](https://github.com/datacarpentry/cloud-genomics).

After some correspondence, it was agreed that the next step should be scheduling a meeting to discuss the changes they had in mind and helping them understand the broader context of integration between the different DC genomics lessons before they sunk a lot of time in.

However, the ball was dropped and the meeting was never scheduled.

Naupaka reached out again in late Fall 2025 to try and schedule a meeting, but has not heard back yet.

- [ ] **Action Item:** Naupaka will follow up again on the email thread (and include Sehrish) to see if they are still interested. If so, he will try to coordinate a meeting between Ben, Emily, and the current DC cloud genomics maintainer Nil Mu [@NilaBlueshirt](https://github.com/NilaBlueshirt) and whichever members of the DC Genomics Curriculum Committee as can attend.

## ReferenceLinks

- https://github.com/datacarpentry/curriculum-advisors
- https://carpentries.slack.com/archives/C9N1K7DCY
