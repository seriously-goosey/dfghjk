# G37 Garage — Skate Shop Edition (Android-friendly PWA)

The interface uses a skate-shop visual theme with a fixed left-side category toolbar on desktop. On smaller screens, the toolbar becomes a compact horizontal navigation strip so the content remains usable on Android.

## Included
- Vehicle profile and odometer
- User-configurable mileage-based maintenance schedule
- Service history with date, mileage, notes and cost
- Modification planner with planned/purchased/installed status, URLs and photos
- Expense tracker
- G37 resource links and saved links
- Local JSON backup and restore
- Installable Progressive Web App shell and offline app shell

## Install on Android
1. Host the contents of this folder on an HTTPS static host (for example, your own web hosting or a static-site host).
2. Open the hosted URL in Chrome on Android.
3. Use Chrome's menu > **Install app** or **Add to Home screen**.
4. Open the installed app and enter your odometer and service history.

A local file opened directly from Downloads is not installable as a PWA. HTTPS hosting is required for service workers and installation.

## Data and notification limitations
- Records are stored in browser local storage on that device. They are not synced to a cloud account.
- Use **Vehicle > Export backup (JSON)** regularly and before changing phones or clearing browser data.
- Mileage reminders are calculated when the app is opened/used and based on the odometer value you enter. This first version does not read the car's odometer automatically.
- Browser notifications require permission and generally need the app/browser to run. Reliable scheduled background notifications require a native Android app or a push-notification backend.
- Uploaded modification photos are stored locally in browser storage; keep image files modest in size.

## Vehicle-specific accuracy
The app is pre-labelled for a 2008 Infiniti G37 Sport Coupe. Confirm drivetrain, transmission, market, current mileage, severe-service use and the factory maintenance schedule for your exact vehicle. Intervals are editable; no interval is represented as an official Infiniti specification.


## Skate Shop × Motorsport redesign (red / balanced)
This edition refreshes the visual layer with a red motorsport accent, graphite surfaces, skate-shop typography and detailing, a fixed desktop sidebar, and a compact horizontal mobile navigation. Existing application storage key and record structures are preserved, so existing browser-local data should remain available when you replace the app files at the same origin. The service-worker cache name is versioned to prompt the updated app shell to load.
