### Updates

So, I have been testing how well AI (LLMs) can be used for auto-cropping questions in PDFs,
similar to the "Prompt AI" feature on the generate answer key page.

The result is that it doesn't work consistently.
The same input prompt that worked once may fail at other times.
This is for consistently structured PDFs.
For inconsistent PDFs, it rarely works.

There are AI models specifically trained to detect layouts, and such models would perform quite well for this task.
The problem is that those models are paid, although some can be used locally on PCs/laptops.

I will revisit "auto-cropping using AI" after a few months.

I will be working on v3 of PDF2CBT starting today, which might take weeks to months.
So there will hardly be any updates during this time, apart from fixes (or small features).

---

### Future of PDF2CBT, v3!

Unlike the update from v1 to v2, v3 will be a fundamentally large update.

As of v2, PDF2CBT is basically a static website.
The server sends webpage files to your browser, which are then loaded.
Everything you do is stored locally on your device (in the browser).
There is no backend/server to upload data to or a database to load from.

This will change in v3, as a database will be added, along with desktop and android app versions so that tests can be managed easily on your local drive without the upload/download process.


**What will be added/changed in v3:**

1. **Test Solutions**:

    Ability to optionally add solutions (text/latex/image/video) to test.
    I don't think there is a need to explain why this is useful.

2.  **A Database of Test Data**:

    Test Maker's data (cropper data, question details, etc.) will be uploaded to PDF2CBT’s online database.
    Let’s call this "test data" for now.


    When an user loads a PDF in Test Maker, PDF2CBT will check whether test data for that PDF exists in the online database.
    - If it exists, the user can load it.
    - If not, the user will have to create it, just like in v1 & v2.

    The data will be uploaded after answer key data is added.

    The plan is to use a vote-based model (similar to Reddit), with a maximum of 10 different test data entries per PDF.
    - Test data with low net votes (e.g., below -5) will be marked for replacement.
    - Newly uploaded test data will start with +1 vote (from the uploader).
    - Users can only upvote after actually attempting the test (to ensure vote quality).

    If a test is loaded from online database and used by an user to give the test, then only after they give the test will they be able to upvote it (this ensures quality vote).

    This feature will help everyone as it shares the test data with each other, making it so that you can focus on giving the mock test instead of preparing it.

    The uploaded data will **not** include PDFs or images (due to storage limits and copyright concerns), so you will still need to upload PDF (locally).

    Uploaded test data will include a tag/badge (username) of the creator.

    Some PDFs will have special test data when uploaded by select special users (initially just me).
    These will not use the voting system as test data by these users should be accurate.

3.  **Storing and managing tests (zips etc) on local drive**:

    Test ZIP files will be stored locally, allowing you to add, modify, and manage tests directly.
    The zip files can then be loaded automatically when it is required (like in question preview of results page).
    This removes the upload/download pipeline from v2 and improves backup/export usability.

4. **Robust backup/restore (import/export) feature**:

    Thanks to point 3 above, PDF2CBT's state (test datas, settings, results etc) can be fully backed up and restored.
    This is very useful for syncing across devices.
    Users can manually transfer backups or use services like Google Drive or OneDrive for periodic syncing.

5. **Ability to Load Tests Hosted by Others**

    Users will be able to load tests hosted externally.

    Say if a person (or a group of people) store test zips in the required structure in a public github repository (repo).
    Tests from this repo can be viewed and loaded in PDF2CBT by just adding the repo url (let's call this bucket).

    You can add url to a bucket on PDF2CBT, and view (folders, files) and load the test you want.
    The test is then saved to local drive after which you can give the test normally.

    When a test is modified/updated in the bucket, the updated test can be replaced with the old one in local drive.
    Further info like description, notes, version notes (why a test was modified) etc can be added too.

    A script/guide on how to setup such a bucket will be made (along with tools to make it easy to structure it as required by PDF2CBT)

    Buckets can also be hosted on Google Drive (via shared links) for private or larger storage use cases.

6. **Host live (or anytime) test**:

    The plan is to add ability for a group of people to give a test like how it is in test series.

    There will be a "host" who will make the test (and decide stuff related to it like test duration, settings etc) and the host can share the link to others to give that test.
    The host can choose when the test can be given (anytime or auto-starts at a specific time).

    As this test is same for the group of people, the comparative analysis like rank list, user vs toppers comparison etc can be done.
    The host can set which comparisons can be done (for example, some might not like user vs toppers comparison).


As you can see, the features planned for v3 are big (and hence will take time).
Initially, v3 will be released with point 1 to 4 features added, then the rest will be added.

Compared to v2:
Login will be required (Google/GitHub, etc.) to associate users with uploads, votes, and live tests.
No personal data is required, it is just for identification.

**You might have this question now: Will PDF2CBT be pay to use?**

I am not some rich guy, nor a saint.
If not for external funds, I wouldn’t even be able to afford my current tier 3/4 college with my family’s ₹1.2LPA income.
Even the laptop I use is borrowed from a friend.

My rule with this project has always been:
"As long as it doesn't cost me money, I won't be charging money from you."
Free resources will be used for all the features and hence doesn't cost me, which means I won't be charging you.

---

### A subreddit for PDF2CBT

As asked by some, I have made a subreddit, [r/PDF2CBT](https://www.reddit.com/r/PDF2CBT/).

This is a subreddit for discussing, sharing, and helping each other with PDF2CBT.

I will also be sharing features I will/am working on so that I can let you all know and get some opinion/feedback during development of that feature
