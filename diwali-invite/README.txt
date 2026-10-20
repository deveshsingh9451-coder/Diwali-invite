DIWALI 2026 — THE MEMORY FILES (invitation website)
=====================================================

WHAT'S IN THIS FOLDER
  index.html   the whole site (design + text + logic in one file)
  assets/      your photos (memory_01..10.jpg) and video clips

PREVIEW
  Double-click index.html. It opens in your browser and works offline
  (the fancy fonts need internet, but the site still works without them).


EDIT THE DETAILS (2 minutes)
  Open index.html in Notepad / VS Code and find the block near the top of
  the <script> that says  "EDIT THESE".  Change:

    hostLine   -> the big announcement line
    dateText   -> the date shown on screen
    startISO   -> real date & time (drives the countdown + calendar button)
    venue      -> your address
    time       -> e.g. "7:00 PM onwards"
    dressCode  -> e.g. "Ethnic & extra"
    whatsapp   -> your number with country code, e.g. "919876543210"
                  (this turns on the green "RSVP on WhatsApp" button;
                   leave it "" to hide the button)

  Captions for each photo are in the  memories = [ ... ]  list just below.
  Video list is in  videos = [ ... ].


PUT IT LIVE FOR FREE (pick ONE)
-------------------------------

OPTION A — Netlify Drop (easiest, no account needed to start, ~1 minute)
  1. Go to  https://app.netlify.com/drop
  2. Drag this whole  diwali-invite  folder onto the page.
  3. You get a link like  https://sparkly-diya-12345.netlify.app
     Share that link on WhatsApp.
  4. (Optional) Sign up free to keep the site permanently and rename it to
     something nicer, e.g.  diwali-at-rahuls.netlify.app
     (Site settings -> Change site name).
  Free limit: 100 GB bandwidth/month — more than enough for a friend group.

OPTION B — GitHub Pages (permanent, free, needs a free GitHub account)
  1. Create a free account at https://github.com
  2. New repository -> name it  diwali-invite  -> Public -> Create.
  3. Click "uploading an existing file", drag in index.html AND the assets
     folder, click Commit.
  4. Repo Settings -> Pages -> Source: "Deploy from a branch" ->
     Branch: main, folder: / (root) -> Save.
  5. After ~1 minute the site is at
     https://<your-username>.github.io/diwali-invite/
  Note: GitHub blocks single files over 100 MB; all files here are under
  that (largest clip is ~42 MB) so it works.

OPTION C — Vercel (free, also drag-and-drop)
  1. https://vercel.com -> sign up free -> "Add New" -> Project
  2. Drag the folder in, click Deploy.
  3. Link looks like  https://diwali-invite.vercel.app


TIPS
  * Keep the folder structure exactly as is (index.html next to assets/).
  * The total upload is ~77 MB because of the videos. If you want a faster
    site, delete the biggest clips from assets/ and remove them from the
    videos = [ ... ] list.
  * clip_07.mp4 and clip_08.mp4 are HEVC (iPhone "high efficiency")
    videos. They play on iPhones and most modern phones but some older
    Android/Windows browsers can't decode them. The site automatically
    hides any clip a device can't play, so nothing breaks. If you want
    them to play everywhere, re-export them as H.264 (e.g. with
    HandBrake, free) and replace the files.
  * memory_11.jpg is a screenshot of the old reveal, not a photo — it's
    not used by the site, you can delete it.
  * The background music is a tiny synthesized loop generated in the
    browser — no copyrighted song, so no takedown problems.
