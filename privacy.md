# MedTrack Privacy Policy

_Last updated: 7 April 2026_

MedTrack ("the app", "we", "our") is an iPhone application that helps you track medication dispensing schedules and remaining supply. This policy explains what information the app handles and how it is stored.

## Summary

**MedTrack stores all of your data on your device.** It does not have a backend, does not transmit your personal information to any server we operate, and does not use any analytics, advertising, or tracking SDKs.

## Information we handle

### 1. Medication data you enter
When you add a medication, MedTrack stores the following on your device:
- Medication name and optional nickname
- Dispensing quantity, unit, and refill interval
- Dose schedule times and quantities
- Dose log entries (time and quantity taken)
- Dispense records (date, quantity, optional cost, optional explicit next-dispense date, optional note)
- Notification preferences
- Tracking mode (whether the medication is tracked in MedTrack or linked to Apple Health)

This information is stored in a private SwiftData database inside the app's sandbox container. It is included in your device's encrypted iOS backups (iCloud or local) if you have those enabled, but MedTrack itself does not sync or upload it.

### 2. Apple Health integration (optional)
If you choose to link a medication to Apple Health, MedTrack uses the iOS 26 HealthKit Medications API to read:
- The list of medications you have explicitly granted the app access to
- Dose events (scheduled and taken) for those medications

You control which medications MedTrack can see via the standard Apple Health per-object authorization prompt. You can revoke access at any time from Settings → Health → Data Access & Devices → MedTrack.

**MedTrack does not write any data to Apple Health.**

### 3. Medication name lookup
When you type a medication name in the Add Medication form, MedTrack first searches a bundled list of approximately 150 common US medications that ships with the app. If your query doesn't match any bundled entries, MedTrack sends the query text to the U.S. National Library of Medicine's public RxNorm API (`rxnav.nlm.nih.gov`) to fetch autocomplete suggestions.

The RxNorm API request contains:
- The text you typed into the name field

The RxNorm API request does NOT contain:
- Your name, email, device identifier, IP is visible to NIH as for any HTTPS request but we don't attach any other identifier
- Any other personal information
- Any other data about your medications, doses, or usage

The RxNorm API is operated by the U.S. National Library of Medicine (NIH). Their terms of use: <https://lhncbc.nlm.nih.gov/RxNav/TermsofService.html>

### 4. Local notifications
MedTrack schedules local notifications on your device for dose reminders, low-supply alerts, and dispense-day reminders. These notifications are generated and delivered entirely on your device by iOS. No notification data is sent to any server.

## Information we do NOT collect

- We do not collect analytics, telemetry, crash reports, or usage data.
- We do not use advertising networks, third-party SDKs, or trackers.
- We do not collect your Apple ID, email, phone number, or contacts.
- We do not collect location, photos, microphone, or camera data.
- We do not have user accounts — there is nothing to log in to.

## Data sharing

We do not share, sell, rent, or disclose any data to third parties. Because MedTrack does not send your data to any server we operate, there is no data for us to share.

## Data retention and deletion

Your data stays on your device until you:
- Delete a medication, dispense record, or dose log from within the app, or
- Delete the app from your device (which removes the entire database)

To export or review your data before deleting, you can use iOS's built-in backup mechanism.

## Children

MedTrack is not directed to children under 13 and does not knowingly collect any information from children.

## Security

Because data never leaves your device, the primary security boundary is your device itself. We rely on iOS's standard app sandboxing and file system encryption. If you lock your device with a passcode or biometric, your MedTrack data is encrypted at rest.

## Changes to this policy

If we make material changes to this policy, we will update the "Last updated" date at the top. Significant changes will be called out in a release note.

## Contact

For privacy questions or data requests, email: **[jog_soffit_7e@icloud.com]**

_(Replace this with your actual support email before publishing.)_
