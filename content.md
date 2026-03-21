### Updates

I (TheMoonVyy) had a throat infection for a week, due to which I was unable to work on PDF2CBT, so there were no updates until yesterday.
Due to this inactivity, some people thought I had stopped working on PDF2CBT with no plans to continue.

Programming is a hobby of mine.
In 2025, I decided to build a project to learn web development. But instead of making basic projects, I thought: why not build a tool I wished existed during my preparation?
That’s how PDF2CBT was created, not only to help me learn but also to help people like you.

I have been working on PDF2CBT since Feb/March 2025 (last year).
Since the first release on 1st April 2025, PDF2CBT has evolved far beyond what I initially expected.

PDF2CBT is currently my only public project and my first one, so I have a strong attachment to it.
There are still many features that can be added, so I don’t plan to stop working on it this year.

That said, whenever I do decide to stop working on PDF2CBT, I will inform everyone instead of going silent.

Due to being sick, the feature mentioned below has been postponed to prioritize other features:

"I am currently working on a feature in the Pattern-Based Cropper that records the steps the cropper takes while searching for, deciding on, and cropping questions. Using this recorded data, we will be able to preview the step-by-step actions in the UI, with speed control, to see exactly how the cropper processes each question. This will help us understand how the cropper works and why it fails to find or crop a question when it is expected to do so."

---

### Upcoming Features

1. I am currently researching and testing how well AI can work for auto-cropping. The plan is to add a feature similar to the **Prompt AI** feature in the **Generate Answer Key** page. These are the two approaches I am testing:
  - Prompting AI with the test PDF, along with JSON data (which will be created automatically by test maker) containing text, images, etc., and their coordinates. This gives AI layout context, allowing it to output crop coordinates of questions along with question info (type, marks, etc.). This would be the best possible cropping feature if it works, as it would make the process truly automatic. However, AI models especially free ones have context limitations, so testing is focused on feasibility and limits.
  - If the above approach is not feasible, then prompting AI with just the PDF to generate a Pattern-Based Cropper's config specific to that PDF will be the way to go.
  - I might add both the above options to make it flexible.
2. App version (initially for desktop) of PDF2CBT. Currently, PDF2CBT is a website, which means it is restricted by browser limitations when accessing local files, external links (like Google Drive), etc. As an app, these restrictions will be removed, allowing automation in the download/upload pipeline, direct file access and managing the tests in local drive.

I have postponed the **Shuffle Questions** feature planned for the Test Interface.
This is because it needs to be implemented alongside support for UGEE (multiple section groups like SUPR & REAP) and BITSAT (bonus section), since all of these require changes to the data structures across all pages.

---

### A subreddit for PDF2CBT

As asked by some, I have made a subreddit, [r/PDF2CBT](https://www.reddit.com/r/PDF2CBT/).

This is a subreddit for discussing, sharing, and helping each other with PDF2CBT.

I will also be sharing features I will/am working on so that I can let you all know and get some opinion/feedback during development of that feature
