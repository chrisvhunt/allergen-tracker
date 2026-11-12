ALLERGEN TRACKER: STANDALONE TEST VERSION
==========================================

What's in this folder
- index.html             The app
- manifest.webmanifest   App name and icons for the Home Screen
- sw.js                  Lets the app open with no internet connection
- icons/                 App icon
- splash/                Launch screens for current iPhone sizes
- .nojekyll              Tells GitHub Pages to publish the files as-is
                         (hidden on some PCs; that's fine)

Upload the folder whole. Don't rename or move files inside it.


PART 1: PUT IT ONLINE (you, on your PC)
---------------------------------------
Pick ONE of the two options below. GitHub Pages is free and permanent.
Netlify Drop is quicker to start.

OPTION A: NETLIFY DROP (about 5 minutes)
1. Unzip this file. You'll have a folder named "allergen-tracker".
2. On your PC, go to https://app.netlify.com/drop
3. Drag the "allergen-tracker" folder onto the page.
4. Netlify gives you a web address, for example
   https://something-random-123.netlify.app
5. Click the option to claim the site and sign up for a free Netlify account.
   Unclaimed sites are deleted, so do this right away.
6. Optional: in Netlify, go to Site configuration > Change site name and
   pick something easier to type, e.g. allergen-tracker-test.netlify.app

Updating later: in your Netlify site, open Deploys and drag the updated
folder onto the drop area. Before you do, open sw.js in Notepad and change
the version (currently "at-v2") to the next number, e.g. "at-v3", so
testers' phones pick up the new version.

OPTION B: GITHUB PAGES (about 10 minutes, free, no expiry)
1. Create a free account at https://github.com and sign in.
2. Click the + at the top right, then "New repository".
   - Repository name: allergen-tracker
   - Choose "Public". Free accounts can only publish Pages from
     public repositories. Testers' data is still private: it never
     leaves their phones. Only the app's code is public.
   - Click "Create repository".
3. On the new repository page, click "uploading an existing file".
4. Open the unzipped "allergen-tracker" folder on your PC, select
   EVERYTHING INSIDE it (Ctrl+A), and drag it onto the GitHub page.
   Drag the contents, not the folder itself, so index.html ends up at
   the top level. The "icons" and "splash" folders upload with their
   files inside.
5. Scroll down and click "Commit changes". Wait until all files are listed.
6. Click "Settings" (top of the repository), then "Pages" in the left menu.
7. Under "Build and deployment" > "Source", choose "Deploy from a branch".
   Under "Branch", choose "main" and "/ (root)", then click "Save".
8. Wait 1 to 10 minutes, then refresh the Pages settings screen. It will
   show "Your site is live at"
       https://YOUR-USERNAME.github.io/allergen-tracker/
   That's the link to send testers.

Updating later on GitHub:
1. Change the version in sw.js (e.g. "at-v2" to "at-v3").
2. In the repository, click "Add file" > "Upload files", drag in the
   changed files (usually index.html and sw.js), and click
   "Commit changes". Files with the same name are replaced.
3. The site updates within a few minutes. Testers get the new version the
   next time they open the app with internet.

Troubleshooting on GitHub Pages:
- Page says 404: check that index.html is at the top level of the
  repository, not inside an "allergen-tracker" subfolder. Also wait a few
  more minutes after the first publish.
- No icon or launch screen: make sure the "icons" and "splash" folders
  uploaded. Testers who installed before the fix should delete the
  Home Screen icon and add it again.


PART 2: INSTALL ON A TESTER'S IPHONE (the tester, about 1 minute)
-----------------------------------------------------------------
Send the tester the web address, then they:
1. Open the link in Safari. Other browsers can add to the Home Screen
   too, but Safari is the most reliable.
2. Tap the Share button. On iOS 26 and later, tap the ··· button first,
   then Share.
3. Scroll down and tap "Add to Home Screen".
4. Leave "Open as Web App" turned on and tap "Add".
5. Open Allergen Tracker from the Home Screen icon.

The app also shows these steps on screen the first time it's opened in
Safari.


WHAT TESTERS SHOULD KNOW
- No account needed. Everything is saved privately on their own iPhone.
  Nothing is sent to you or anyone else.
- It starts with sample data. Tap "Start my log" to clear it and begin.
- After the first open, it works without internet.
- Deleting the Home Screen icon deletes their data. To keep it safe, use
  Allergens tab > Back up data and save the copied text in Notes.
- It spots patterns. It doesn't diagnose allergies or replace a doctor.
