# MedTrack Support

MedTrack helps you track medication dispensing schedules, dose logs, and remaining supply on your iPhone.

## Contact

For bug reports, feature requests, or general questions, email: **[jog_soffit_7e@icloud.com]**

Please include:
- Your iOS version
- Your iPhone model
- The version of MedTrack (Settings → General → iPhone Storage → MedTrack)
- A clear description of what happened and what you expected

## Frequently asked questions

### Why does MedTrack need access to Apple Health?
Only if you choose to track a medication via Apple Health. In that mode, MedTrack reads the dose events you log in the Health app to calculate how many doses you have remaining. You control which medications MedTrack can see via the standard Health permissions prompt, and you can revoke access at any time.

### Does MedTrack write my doses to Apple Health?
No. The Apple Health Medications API is read-only for third-party apps. Only the Apple Health app itself can create medication dose samples.

### Where is my data stored?
Entirely on your device. MedTrack has no server and does not sync your data to any cloud service we operate. Your data will be included in your iPhone's iOS backups if you have those enabled (iCloud or local).

### Why does my low-supply calculation seem off?
MedTrack calculates remaining supply as (total dispensed) minus (total doses taken). If you forget to log a dose, or log a dose with the wrong quantity, the calculation will be off. You can edit dose logs by tapping the row in the "Today's Doses" section on a medication's detail page.

For medications linked to Apple Health, the calculation uses the dose events logged in Health. If you log a dose in Health and the Supply gauge doesn't update, pull down on the dashboard to refresh.

### How do I get reminders for my doses?
Add a medication with a daily schedule — each dose time you add becomes a local notification. Make sure notifications are enabled for MedTrack in Settings → Notifications → MedTrack.

### What is the "Next Dispense" date?
By default, MedTrack calculates the next dispense date by adding your configured refill interval to your most recent dispense. If your pharmacy has printed a specific "next available" date on your prescription, you can enter it in the Record Dispense dialog — MedTrack will use your explicit date and schedule the refill reminder for that day.

### What is the "Track via Apple Health" option?
This is an alternative to tracking schedules and doses inside MedTrack. If you already manage a medication's schedule and reminders in the Apple Health app, you can link it in MedTrack so the supply calculation uses your Health dose logs. In this mode, MedTrack only tracks the pharmacy dispenses (Health doesn't track those); the dose schedule and reminders live in Apple Health.

### Does MedTrack work offline?
Yes, entirely. The one exception is medication name autocomplete, which uses a bundled list first and then falls back to the RxNorm API when online. If you are offline and the bundled list doesn't contain your medication, just type the full name manually.

### How do I delete my data?
To delete a single medication and all its records, open the medication's detail screen, tap the pencil (edit), and tap "Delete Medication" at the bottom. To delete everything, delete the app from your device — this removes the entire private database.

### Will MedTrack be on iPad?
MedTrack builds for iPad and supports iPad multitasking. The UI is designed for iPhone, so it appears centered on iPad rather than fully responsive. An iPad-optimized layout is planned for a future release.

## Privacy

See the [privacy policy](./privacy.html).
