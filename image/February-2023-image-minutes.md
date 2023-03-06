## 2023-02-22 CAC-DC-Image Meeting

* Date and time: [Wednesday, February 22, 2023, 20:00 UTC](https://www.timeanddate.com/worldclock/fixedtime.html?msg=CAC+Meeting+DC+Image+Processing&iso=20230222T20&p1=1440&ah=1)

### Sign-in

* Erick Ratamero (Timekeeper)
* Ulf Schiller (Notetaker)
* Marianne Corvellec
* Sunil Shende

### Regrets
* Josh Moore

### Agenda

* Discuss options (and weigh in) for fixing exercise where RGB image is converted/loaded into grayscale (see GitHub issue [#249](https://github.com/datacarpentry/image-processing/issues/249#issuecomment-1424285829))

    - image `data/sudoku.png` is an RGB-A image with a trivial alpha channel; alpha channels are never explained in the lesson; image shape (4 channels) may be problematic (confusing to learners); Marianne recommends re-saving the image as pure RGB
    - do we want to load it as grayscale? may not be very robust; `mode="L"` is dependent on the backend; possible solution: load image as RGB and do an explicit conversion; difference between loading with imageio and skimage.io (image is uint8 when read with imageio, whether as RGB or as grayscale; it is also uint8 when read with skimage.io by default, but it is float64 when passing `as_gray=True`); maybe add an explicit explanation/callout to explain difference in data types (dtype in numpy language, pixel types as Erick calls them)
    - Erick: discussion of alpha channels and image formats is in purview of CAC; rather not talk about alpha channels (avoid cognitive overload); discussion of pixel types might make sense
    - clarification from Marianne: change the image file to RGB; redo the exercise with integer dtype (0-255 range); changing `mode="L"` is not critical;
    - Erick: recommendations we can make: images should not use alpha channels; different formats should be discussed;

* Standardize handling of import statements in Jupyter notebooks?  (see Github issue [#196](https://github.com/datacarpentry/image-processing/issues/196))
    * Ulf: would it make sense to have all imports in the first cell of the notebook?
    * Marianne/Erick: Maybe have a discussion with maintainers of others lesson.

* "Edge detection" bonus episode (see Github issue [#241](https://github.com/datacarpentry/image-processing/issues/241))
    * Erick: there is value in bonus materials; however, if the bonus episode differs to much in style/level of the other episodes it may not be a good fit for the lesson.
    * Question from Sunil: Is it a lot of effort to maintain the bonus episode?
    * Marianne: This extra episode has already drifted: There are issues that need to be addressed. At the moment the extra episode is not self-contained/standalone. Rather move it to an upcoming (more specialized or more advanced) follow-up lesson.
    * Ulf summary of discussion: Extra episode needs some effort to bring up to standards; consensus that it is better to remove lesson and keep it in the backlog.

* Informational item: Transition to Workbench is underway
    > The second stage of the beta phase is now live. This is a big milestone because this is the portion of the beta phase where our community of contributors will get a chance to interact with and use the Workbench in our live lessons before we transition all of our lessons to use the new infrastructure in May 2023.
    * https://carpentries.org/blog/2023/02/dovetail-15/
    * https://carpentries.org/blog/2022/05/workbench-beta/

* Q from Sunil: Has there been any discussion on video processing?
    * Marianne: Time dependent image analysis would be very interesting.
    * Erick: Tracking is often included in other teaching of image processing: https://erickmartins.github.io/training/ImageAnalysis.html
    * Ulf: not sure what the mechanism would be to solicit new curriculum materials (Q for consideration by Carpentries Core Team?)

* Adjourn
    * next meeting is planned on [May 31, 2023, 20:00 UTC](https://www.timeanddate.com/worldclock/fixedtime.html?msg=CAC+Meeting+DC+Image+Processing&iso=20230531T20&p1=1440&ah=1)
