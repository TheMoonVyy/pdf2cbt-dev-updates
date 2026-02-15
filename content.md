### Updates

TheMoonVyy here, now that my 1st semester exams are over, I can focus on upcoming features for a week so expect updates.

---
### Upcoming features
1. Currently I am working on a feature in Generate Answer Key page which will create a prompt users can copy and paste it to an AI (like chatgpt, gemini etc) along with their answer key pdf or screenshot.
  - The prompt will prompt the AI to extract the answers from PDF/Image and provide back a json output which users will have to copy and paste it back to generate answer key.
  - The page will then validate the answer key data and create the answer key in the format needed by PDF2CBT.
  - The prompt and AI's output format is being designed to be minimal so that the prompt context is not lost to the AI.
  - I have a similar idea for creating Pattern Based Cropper's Config using prompt + pdf.
2. Add a ```Shuffle Questions``` button inside the ```Test Interface``` to shuffle questions within their respective sections.
3. Add an ```Offset Test Duration``` option in UI Settings of Test Interface. This will visually extend the countdown timer by the given offset while keeping the real test duration unchanged.
  - For example, if the test duration is set to 150 minutes and the offset is 30 minutes, the timer will start from 180 minutes.
  - The countdown will run normally until it reaches 30 minutes remaining, at which point the test will automatically submit because the internal duration is still 150 minutes.
  - This is a purely visual feature intended to create a psychological buffer without affecting actual timing or evaluation logic.

---
### A subreddit for PDF2CBT

As asked by some, I have made a subreddit, [r/PDF2CBT](https://www.reddit.com/r/PDF2CBT/).

This is a subreddit for discussing, sharing, and helping each other with PDF2CBT.

I will also be sharing features I will/am working on so that I can let you all know and get some opinion/feedback during development of that feature
