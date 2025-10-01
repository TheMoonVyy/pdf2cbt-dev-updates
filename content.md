## A subreddit for PDF2CBT

As asked by some, I have made a subreddit, [r/PDF2CBT](https://www.reddit.com/r/PDF2CBT/).

This is a subreddit for discussing, sharing, and helping each other with PDF2CBT.

I will also be sharing features I will/am working on so that I can let you all know and get some opinion/feedback during development of that feature

---

## (Under Development) Text Pattern Based Auto Crop for PDF Cropper

This is a feature I have been working on for weeks and finally it will be released today (1st oct) or tomorrow (2nd oct)!
(A video showing it in action is below)

The current PDF Cropper's process is manual, it requires users to manually crop the questions.
Manual cropping made it possible to crop a wide range of PDF formats but its strength is also its weakness, it is tedious to manually crop.

To solve this problem, we can make use of text patterns in the PDF to determine the location of questions.
This is what Pattern Based Cropper is for, but for this, we need know what the patterns are and instead of going with a big general case of patterns, we can go with specific patterns for a given pdf format.

With this in mind, I came up with this **config based approach**, where you create a pattern config first and use it to crop pdfs following that config (which will be the case if pdf is created by same people and they are using same template/format).
I have added a lot of options to the config for flexibility.

I will be providing some popular pattern configs for users to select from (and create a new one based on it if needed) and if you want to include more in the list you can let me know.

Here's the video showing how the config looks and pattern based cropper in action (explanations will be there when it is released (in instructions/docs and in video)).

@[youtube](SKwI29w3c3U)


Feel free to share your thoughts by commenting in this [github discussion](https://github.com/TheMoonVyy/pdf2cbt/discussions/122) or this [reddit post](https://www.reddit.com/r/PDF2CBT/comments/1nv141x/text_pattern_based_auto_crop_for_pdf_cropper/).
