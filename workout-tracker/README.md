# Workout Log (iPhone, offline, local-only)

A simple workout tracker you add to your iPhone Home Screen. Type the exercise, reps and
(optionally) weight in kg, then tap **Add set**. Sets are grouped by exercise for each day,
and **History** lists every past day.

**Your data stays on your phone.** It's saved in the app's local storage and never sent anywhere.
The web address is only used to download the app files once. After that it works offline.

## Features
- Log exercise, reps and weight (kg, optional). Sets are numbered automatically.
- Daily totals: exercises, sets, reps, volume (reps × kg).
- "Repeat last set" button. The last weight used for each exercise is filled in for you.
- Exercise name suggestions from what you've logged before.
- Tap a set to edit or delete it.
- Use ‹ › to go back and log a day you missed.
- History of all days. Tap one to open it.
- Export and import a JSON backup.

## Install on your iPhone
1. On GitHub, open this repo → **Settings → Pages**. Under *Build and deployment*, choose
   **Deploy from a branch**, pick the branch and `/ (root)`, then **Save**.
2. After a minute, open `https://<your-username>.github.io/<repo-name>/workout-tracker/` in **Safari** on your iPhone.
3. Tap **Share → Add to Home Screen → Add**.
4. Open **Workouts** from your Home Screen. It runs full-screen and works offline.

> Removing the Home Screen icon, or clearing Safari's website data, deletes the logged workouts.
> Use **History → Export backup** from time to time.

## Updating the app
After changing `index.html`, bump `VERSION` in `sw.js`. The phone picks up the new version the
next time the app is opened with an internet connection.
