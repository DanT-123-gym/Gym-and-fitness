# Tudor Training — standalone app

## What is included
- Workout planner with two upper-body-priority sessions.
- Set-by-set weight and rep logging.
- Shared progress dashboard and workout history.
- Voice input where the browser supports SpeechRecognition, plus typed input.
- Soreness check-in and conservative workout-adjustment suggestions.
- Rest timer.
- Equipment category directory and personal machine notes.
- JSON backup export/import.
- PWA manifest and service worker for installability and offline app shell.

## Important limitations
- The Tudor Grange equipment directory is a starter list of equipment categories, not a verified live inventory of every machine or attachment.
- Voice recognition availability varies by browser/device. On iPhone, Safari may not expose browser speech recognition consistently; keyboard dictation is an alternative.
- App data is stored locally in the browser on that device. Export a JSON backup regularly. It does not automatically sync between devices.
- This is a workout organiser, not a medical tool. Pain or possible injury should not be treated by simply swapping exercises.

## Publish it so it can be installed on iPhone
A PWA needs to be served from a secure HTTPS website. You cannot install the ZIP directly as a Home Screen app.

### Simple route: GitHub Pages
1. On a computer, create/sign in to a GitHub account.
2. Create a new repository, for example `tudor-training`.
3. Upload `index.html`, `manifest.webmanifest`, `sw.js`, and `icon.svg` from this folder to the repository root.
4. In the repository, open **Settings → Pages**.
5. Under Build and deployment, choose **Deploy from a branch**, select `main` and `/ (root)`, then Save.
6. Wait for GitHub Pages to publish the site. Open the URL shown in Pages settings.
7. On your iPhone, open that URL in **Safari**.
8. Tap the Share button → **Add to Home Screen** → optionally enable **Open as Web App** if shown → **Add**.

You can also use another static HTTPS host. Keep all four files together in the published site.

## Using it
- Open Train, choose Gym A or Gym B, enter the actual weight and reps for each set, then Save set.
- Talk lets you type or dictate how you feel. Review the suggested adjustment before using it.
- Tools contains the rest timer and equipment directory.
- Progress shows saved results and lets you export/import a backup.
