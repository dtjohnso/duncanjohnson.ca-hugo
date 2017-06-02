+++
title = "student work showcase baptist history timeline"
date = "2013-12-06"
slug = "2013/12/06/student-work-showcase-baptist-history-timeline"
Categories = []
+++

[![Baptist History Timeline project](/images/2013/11/timeline.png)][timeline]

This semester, students in my Baptist History class were responsible for a group project to construct an [online timeline][timeline] of key events in the history of the Baptist movement. It has been rather interesting to watch this project develop as the students submitted events and presented their findings to the class. Since my students submitted their final entries this week, I thought I'd share their work, write down my observations on the project as a classroom assignment, and note some ideas I've had for ways to use this in the future.

<!-- more -->

## Thoughts on Educational Value

As an assignment, I found that this was a useful project in several ways.

1. It created interest in the course by allowing students to explore areas of interest. Some of my students said that they didn't like the class at first, but as a result of the project it was now one of their favorite classes.
2. It encouraged my students to read widely from the literature.
3. The atomistic nature of the assignment (30 separate timeline entries submitted in smaller assignments over the semester) was less intimidating than a 10-20 page paper on a single topic. This makes it an interesting project for a survey class, as it allows students with no prior knowledge or interest to expand their knowledge in any direction they choose.
4. It forced my beginning history students to grapple with questions of significance as they analyzed historical events. In selecting events for their timeline contributions, students had to decide whether an event was truly significant for the grand story of the Baptists throughout history. Sometimes they made good choices and sometimes they didn't, but the exercise itself helped to introduce them to the basics of selecting and evaluating evidence.

Of course, there are some inherent weaknesses too.

1. Because it focuses on dates and data, the project doesn't require the construction of a coherent argument or narrative. My goal was to supplement this deficiency through reading assignments and lectures, and to some extent student performance on assessments suggests that this actually worked.
2. Because students come to the project with limited knowledge, their choices tend to reflect inherent prejudices and/or emphases from class lectures.
3. Because students were required to submit a specific quota of events, they did not always select truly significant events. I tried to reflect that in my marks for their assignments, but overall I'm happy with the results of their work.
4. Because it emphasizes finding separate events, it tends to result in superficial knowledge rather than deep comprehension.

There are probably other observations I could make on the effect of this assignment, but this is enough for now. In summary, I thought it was a worthwhile project and a useful student assignment which I'll repeat in future offerings of this class.

## Ideas for Future Implementation

This sort of project is something I've done by myself a few times before. Examples of my own efforts this way can be found on my [Projects page](/projects/). As I review the events which my students chose for their contributions, there are a number of things I would probably do differently.

I have plenty of ideas for things that I could do with this project at some later date. These ideas roughly break down into three areas: 1) pedagogy, 2) content and 3) technical.

### Pedagogy

One oversight in my project definition was any reference to grammar, spelling, and capitalization. I shouldn't need to worry about this at this level, but the simple reality is that my students tend to struggle with these things. This should factor into their marks, but it didn't for this class because my expectations were too idealistic.

### Content

At some point, I'd like to take my students' contributions, edit them, and put them into a fresh dataset that represents my own perspective on the history of Baptists. If I ever do this, I will keep the appropriate "Contributor" attribute in the dataset to acknowledge the original work of my students. In many ways, their submissions exhibit a level of passion that my own timeline projects have never had.

If I ever do that, here are some things I would change:

* I'd place less focus on individuals and organizations and more focus on concrete events. Although many of the individuals/organizations my students selected are important, I'm not sure that representing the duration of some of these peoples' lives is truly significant for the full story of the Baptists. Some individuals truly were significant over the course of their life, such as Charles Spurgeon and William Carey. Others, though, are perhaps better remembered for a few accomplishments than for a lifetime of significant efforts, such as perhaps Benoi Stinson or Sarah Cummings.
* I'd reorganize the events under a more uniform set of categories that are defined in terms of specific chronological periods. At the beginning, I defined only three simple categories for my students: "English Particular Baptists," "English General Baptists," and "Baptists in America." These categories are really only useful for telling the story of Baptists from their founding in the 1600s until around the end of the 18th century. After that, those categories become rather clunky. For instance, "Baptists in America" would probably make more sense if I changed it to "Baptists in America before 1845." After 1845, I'd need to create separate categories for Northern and Southern Baptists, as well as other groups of Baptists that developed after that time.
* I'd edit my student entries to only include the most significant entries. In other words, in producing my own dataset based on their contributions, I'd filter out the submissions that where significance is questionable. I'd still retain their work in a data file that includes all the entries made by that particular class, but not all of those entries would make it into my edited version of the dataset.
* I'd also supplement student contributions to correct for lacunae. My students did some admirable work on this project, and in many cases identified truly significant events to display. However, they still missed a few truly significant things, either due to a lack of knowledge or interest. For instance, one of my students included several of Adoniram Judson's wives, but not one of my students thought to create an entry for Adoniram Judson himself.

### Technical

This project depends on code (specifically, the [Simile Exhibit Timeline plugin][simile]). As a result, there are always technical things that need maintenance, as well as technical opportunities that could be explored. Someday, here are some things that I'd love to get done to make this sort of project more useful.

* Change the lens design to include links to copies of the original text of a document when available in a similar way to the wikipedia links.
* Implement multiple datasets so the same code can be reused for each class where I give this as an assignment.
* Upgrade the timeline code to take advantage of improvements in Simile Exhibit 3.0 (or one of the newer implementations that can be found in the [SIMILE Widgets Google Group][google-group]). Apparently there are [other projects out there that do similar things][alternatives] (some of which may even work better), but I'm too heavily invested in the Simile Exhibit framework to be interested in switching to an alternate platform right now.
* Develop a better system for submitting entries that supports image upload and supports additional file formats (SVG was a problem). I'm not completely sure how I would set this up. Ultimately, I'd probably need to set up access to Amazon S3 storage, but there's no way to easily incorporate that into my current system where students submit entries via a Google Spreadsheets form and can immediately see the results on the timeline itself.
* Implement geo-code support within the timeline dataset, and then implement functionality to switch between timeline view and map view. Because geo-code data requires advanced technical skills to generate, this is not something I would require students to submit but would be nice to have in edited versions of the dataset.



[timeline]: http://duncanjohnson.ca/Baptist-History/
[google-group]: https://groups.google.com/forum/#!forum/simile-widgets
[alternatives]: http://stackoverflow.com/questions/4700419/alternative-to-simile-timeline-for-timeline-visualization
[simile]: http://simile-widgets.org/
