TUDOR TRAINING — UPDATED APP PACKAGE

CONTENTS
- index.html: the app and its features
- manifest.webmanifest: installable app metadata
- sw.js: offline cache (version bumped for this update)
- icon.svg: app icon

IMPORTANT DATA NOTE
Workout history is stored in local browser storage under the existing key tudor-training-v1. This update keeps that key and adds new optional fields, so the existing browser data is intended to remain compatible. Still export a backup from PBs before updating. Local browser data does not automatically sync between devices.

FEATURES IN THIS UPDATE
- Six main tabs: Week, Train, Talk, PBs, Sport and Home
- Add one-off or weekly repeating calendar entries for gym, runs, sport and rest; edit and delete entries
- Personal best summary based on logged weights/reps
- Equipment selection saved in the Home generator, plus custom equipment notes
- Home workout builder filters exercises against selected equipment and chosen focus/time/effort
- Home workouts can be opened in Train and logged using the existing set logger
- Exercise like/dislike feedback is saved and influences future home workout selection
- Rest timer starts automatically after a saved set when another set remains
- Existing Talk assistant, gym sessions, training history, export/import and equipment directory retained

GITHUB PAGES UPDATE GUIDE
1. Open the current app and go to PBs. Choose Export backup and save the JSON file somewhere safe.
2. Download and extract this ZIP on your computer. Open the tudor_training_app folder.
3. Open https://github.com/dant-123-gym/Gym-and-fitness
4. Check that you are on the main branch. Choose Add file, then Upload files.
5. Upload the five files from tudor_training_app directly into the repository root (not inside a new folder). Allow GitHub to replace the existing files with the same names.
6. Enter the commit message: Update Tudor Training. Choose Commit changes.
7. Wait for GitHub Pages to publish, then open https://dant-123-gym.github.io/Gym-and-fitness/ and refresh.
8. On iPhone, close the installed app fully and reopen it. If it still shows the old version, open the website in Safari and refresh before reopening the Home Screen app.
9. Check the Week, Train, Talk, PBs, Sport and Home tabs. Confirm old workout history is still visible before importing any backup.

ROLLBACK
The existing version can be restored from GitHub's commit history if needed. Do not delete the repository. Keep your exported JSON backup.

LIMITATIONS
- Calendar events and exercise preferences are stored locally in this browser.
- The equipment directory is a broad category guide, not a verified complete inventory of Tudor Grange machines.
- Home exercise selection is rule-based; custom equipment names are saved for your reference, but only equipment types represented in the exercise library can currently unlock matching exercises.
- PBs are calculated from the sets you have logged; they are not independently verified strength standards.
