# MY LIFE PWA v1.3

A free, offline-capable personal iPhone PWA using HTML, CSS, vanilla JavaScript and browser localStorage. No backend or account required.

## Features
- Home dashboard and quick actions
- AED expenses with categories, dates and deletion
- Monthly budgets, spending totals and progress bar
- Date-wise daily planner with completion tracking
- Travel destinations, dates and budgets
- Activity reminders: date, time, category, repeat (daily/weekly/monthly/yearly), edit, dismiss, and delete
- In-app due alerts while the app is open (no background push notifications)
- JSON backup export/import
- Installable PWA manifest and offline service worker

## Publish for free
1. Create a GitHub repository and upload the contents of this folder to the repository root.
2. In repository Settings → Pages, choose **Deploy from a branch**, branch `main`, folder `/ (root)` and Save.
3. Wait for the HTTPS GitHub Pages URL to become available.
4. On iPhone, open the HTTPS URL in **Safari**, tap **Share**, then **Add to Home Screen** and **Add**. On some iOS versions choose **Open as Web App** if shown.

For local desktop testing, run `python -m http.server 8000` from this folder and open http://localhost:8000. Service workers require HTTPS or localhost.

## Privacy and limits
Data is saved only in the current browser/device storage. Clearing Safari website data, changing device or deleting website storage may permanently remove data. Use Settings → Export backup regularly and store backups safely. Import replaces all current records. No account sync or automatic cloud backup. The app is not a secure password vault and does not include HealthKit, background push notifications, live travel booking, or investments in v1.


## Version 1.2: Travel departure alerts
When adding a trip, select the departure date and local departure time. The app automatically displays a reminder 2 hours before that time, including when the reminder falls on the previous calendar day. Existing trips without a departure time remain unchanged; add a new trip with time to use this feature. The reminder is displayed only while the app is open (or when reopened after the alert time). It is NOT a reliable background alarm and cannot guarantee an audible alert while the phone is locked. For important flights also use iPhone Clock or Calendar alarms.

## Version 1.3: Premium interior theme
Redesigned home, finance, planner, travel, reminders and settings screens with premium cards, improved typography, lavender/navy palette and user-selectable Light, Dark and System appearance. Existing localStorage data key remains unchanged. Export a backup before updating.

## Admin customization v1.4
Under More, the admin can add or remove custom informational sections. First login sets a local password for username Sajidpp. This is a local convenience lock, not secure multi-user authorization. Do not put passwords into GitHub. Real access control requires a server.

Version 1.5: Admin custom sections now support Edit and Save Changes, in addition to Add and Delete. Clear old cache or reload after deployment. Local admin login does not protect data against browser users with technical access.

Version 1.6: floating Alarm + button visible on every page, plus Add Alarm in reminders. Opens the existing date/time/repeat activity reminder form. These are in-app reminders, not guaranteed iPhone system alarms while the app is closed.

Version 1.7: foreground audible Web Audio alarm tones (Classic, Gentle, Urgent), Enable Sound, Test Tune, Stop Ringing. iOS requires user interaction to unlock sound; app must remain active. Not a background alarm or push notification.

Version 1.8: Add trip now includes Add travel alarm checkbox, lead-time and tune selector, and Test alarm tune. Saving a trip with the checkbox creates a corresponding reminder. The original automatic 2-hour travel reminder is suppressed for trips with a custom alarm. Alarm audio works only while app is active; iOS background/locked alarms not guaranteed.

## Version 1.9 – Task alarms
The Add Task dialog includes an Add task alarm checkbox, lead-time selector, tune selector and Test Tune. Selecting an alarm requires a task time. Saving creates a linked reminder; deleting the task deletes its linked reminder. Sound requires tapping Enable Alarm Sound and keeping the app active; iOS web apps cannot guarantee a ringing alarm when locked or closed.

## Version 2.0 My Documents
Go to More > My Documents. Upload UAE Emirates ID, passport, Aadhaar, PAN, visas and other files. Files are encrypted in the browser with AES-GCM, using a passphrase-derived key, and stored in IndexedDB on the device. You must remember the passphrase. No cloud sync or server uploads. Export documents individually; the normal JSON backup excludes files. 15 MB per file limit. This is not an audited security product; avoid relying on it as the only copy of irreplaceable identity documents.

Version 2.1: My Documents has a local passkey privacy gate. On first unlock, register a passkey; later unlocks request iPhone Face ID or device passcode when available. This is NOT server-verified WebAuthn; users controlling browser storage or app code may bypass the UI gate. Encrypted document files still require their passphrases. No secure account recovery; removing the passkey may prevent access to the gate. Do not use this as the sole protection for sensitive identity documents.


## Version 2.2 — Professional UI refinement
Refined typography, color palette, dashboard, cards, input fields, modal sheets, navigation bar, dark mode, accessible focus styles and reduced-motion behavior. No intentional change to app data schema. Before replacing GitHub Pages files, export your app backup. Visual changes should be checked on a physical iPhone.

Version 2.3: ML Sajid pp custom branding, Home header logo, new PWA icons, About logo. Safari may cache old icons; remove and re-add Home Screen shortcut if necessary.
