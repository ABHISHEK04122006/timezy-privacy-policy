# Privacy Policy for Timezy

**Application Name:** Timezy (Countdown & Widget)  
**Package Identifier:** `com.timezy.widget`  
**Effective Date:** October 22, 2026<br>
**Last Updated:** November 13, 2026

---

## 1. Introduction

Welcome to **Timezy**. Timezy is an offline countdown and home-screen widget application designed to help you track important life events, milestones, and deadlines.

Your privacy is simple with Timezy: **your data stays on your device**. Timezy does not require account creation, registration, or logins. You can use the application completely anonymously without providing your name, email address, or phone number.

This Privacy Policy explains what information is stored, how it is handled on your device, what permissions are used, and how your privacy is protected. It is drafted with reference to India's **Digital Personal Data Protection Act, 2023 (DPDP Act)** and applicable privacy principles.

---

## 2. Information Stored by Timezy

Timezy only handles information that you choose to enter into the app to manage your countdowns:

### A. Information You Provide
* **Event Details:** Countdown titles (e.g., "Mom's Birthday", "Exam"), optional notes or descriptions, target dates, and optional times.
* **Display Preferences:** Event categories (e.g., Birthday, Anniversary, Work), visual accent themes, widget styles (Liquid Glass, Pure White, Smoked Glass), and seconds counter preferences.
* **Reminder Settings:** Alert timing preferences you select for scheduled notifications (e.g., 1 day before, 1 hour before).

All of this information is stored locally on your device.

### B. Information Timezy Does NOT Collect
* **No User Accounts:** We do not collect names, email addresses, phone numbers, or passwords.
* **No Device Identifiers:** We do not collect IMEI numbers, MAC addresses, Android Advertising IDs (AAID), or hardware identifiers.
* **No Location Data:** Timezy does not access your GPS or network-based location.
* **No Sensor or Media Data:** Timezy does not access your camera, microphone, photos, or contacts.
* **No Tracking or Analytics:** Timezy contains no tracking code, telemetry, or analytics SDKs to monitor your application usage.

---

## 3. How Information Is Stored

All countdown titles, notes, dates, categories, and preferences are stored locally on your device within Timezy's private application storage:

* **Event Database:** Stored locally in a private SQLite database managed by Android Jetpack Room (`countdown_widget.db`).
* **Preferences:** Display settings, styles, and toggles are stored locally using Android Jetpack DataStore and SharedPreferences.
* **Sandbox Location:** All data resides in Timezy's private directory (`/data/user/0/com.timezy.widget/`), protected by Android's application sandbox from access by other apps.
* **Android System Backups:** Android system backup features may handle eligible app data separately, depending on your device settings and the app's backup configuration (`android:allowBackup="true"`). If enabled by the user, Android may include eligible local app data in private device backups (such as Google Drive backups).

---

## 4. How Information Is Used

Information you enter is used exclusively to provide the core functionality of the application:

* **Calculating Countdowns:** Calculating remaining days, hours, minutes, and seconds until your target dates.
* **Home-Screen Widgets:** Rendering your countdowns on your device's home screen in your chosen visual style.
* **Delivering Local Reminders:** Triggering on-device notifications at the specific times you scheduled.

Your information is never used for advertising, user profiling, automated decision-making, or commercial resale.

---

## 5. Data Sharing

Timezy does not directly transmit your countdown events or preferences to external servers. The app does not request Internet permission and does not use cloud synchronization, analytics or advertising services.
Android system backup features may handle eligible app data separately, depending on your device settings and the app's backup configuration.

Timezy does not sell, rent, or trade your data, and does not integrate any third-party tracking, advertising, or analytics SDKs.

---

## 6. Android Permissions

Timezy requests only the minimum permissions necessary to deliver local reminders and widgets:

| Permission | Purpose | How to Manage |
| :--- | :--- | :--- |
| **`POST_NOTIFICATIONS`** *(Android 13+)* | Allows Timezy to show reminder notifications in your notification shade when an event alert triggers. | Can be granted or revoked at any time in **Android Settings > Apps > Timezy > Notifications**. |
| **`SCHEDULE_EXACT_ALARM`** | Allows Timezy to schedule exact reminder alerts using Android's `AlarmManager`, ensuring reminders trigger on time even in battery-saving Doze mode. The app gracefully falls back to standard inexact alarms if exact alarm access is unavailable. | Managed via **Android Settings > Apps > Special App Access > Alarms & reminders** (Android 12+). |
| **`RECEIVE_BOOT_COMPLETED`** | When your phone reboots, Android clears active memory alarms. This permission allows Timezy to automatically restore your upcoming reminders into `AlarmManager`. | Handled automatically by Android at startup; runs locally with no user intervention required. |
| **`VIBRATE`** | Provides gentle haptic vibration when a countdown reminder notification appears. | Controlled by your device's sound and vibration settings. |

---

## 7. Data Retention and Deletion

Because Timezy stores data locally on your device, you have direct control over data retention and removal:

* **Deleting an Event:** When you delete a countdown event inside the app, it is removed from the app's local database. However, separate device backups (such as Google Drive backups created prior to deletion) may retain copies until overwritten or deleted by system backup cycles.
* **Clearing App Storage:** You can delete all your stored data within the app at once by navigating to **Android Settings > Apps > Timezy > Storage > Clear Storage / Clear Data**. This removes all saved events, preferences, and cached widget data from the device.
* **Uninstalling the App:** If you uninstall Timezy, Android removes the application's local database and stored preferences from your device. Separate system backups created previously by your device may retain copies according to your device backup settings.

Because we do not maintain central servers, data deletion happens directly on your device without needing an external request.

---

## 8. Data Security

We take reasonable technical precautions to protect your data through Android's built-in platform security:

* **Sandbox Isolation:** Android's operating system assigns Timezy a unique Linux user ID (UID). Other apps cannot read or access Timezy's private storage.
* **On-Device Encryption:** On supported Android devices, local app data is protected by Android's File-Based Encryption (FBE).
* **Offline Protection:** Because Timezy does not transmit data over the internet or store it on cloud servers, your information is not exposed to server-side data leaks or network interception.

**Please Note:** No mobile application or operating system can guarantee absolute security. Your data's safety also depends on your physical device security, such as maintaining a secure screen lock, PIN, or biometric protection.

---

## 9. Children's Privacy

Timezy is a general-audience utility for managing dates and countdowns. We do not knowingly collect personal information from children under 18 years of age.

* Any information entered into Timezy is stored locally on the device.
* Timezy does not profile users, track behavior, or display targeted ads to anyone, including children.
* Parents and guardians can view, edit, or delete any event entered by a child directly within the app, or clear the app's local storage via device settings at any time.

---

## 10. Your Privacy Rights

Under applicable privacy legislation, including the relevant provisions of India's **Digital Personal Data Protection Act, 2023**, you have choices and rights regarding your data:

* **View and Access:** You can view all information stored by Timezy directly on your screen at any time.
* **Edit and Correct:** You can update or edit any event details, notes, or dates directly within the app.
* **Delete Information:** You can delete individual events within the app or remove all data via device settings (`Clear Storage`).
* **Manage Notifications:** You can disable reminder notifications at any time in Timezy's settings or via Android system settings.
* **Grievance Redressal:** You have the right to contact the publisher regarding privacy queries or concerns as outlined in Section 11.

*Note on Phased Implementation:* The provisions of India's DPDP Act, 2023 and the DPDP Rules are being brought into force in phases by the Government of India. Timezy aims to uphold statutory privacy principles as applicable provisions become legally operative.

---

## 11. Contact and Grievance Redressal

If you have questions, feedback, or privacy-related concerns regarding Timezy, you may reach out to our designated contact:

* **App Name:** Timezy
* **Package Name:** `com.timezy.widget`
* **Publisher / Developer Name:** Prayas
* **Grievance Contact Person:** Prayas
* **Privacy Contact Email:** [prayasingale0909@gmail.com](mailto:prayasingale0909@gmail.com)
* **Postal Address:** [Pending - to be provided by publisher upon commercial distribution if required]
* **Project Repository:** [https://github.com/ABHISHEK04122006/Timezy-Application](https://github.com/ABHISHEK04122006/Timezy-Application)
* **Public Privacy Policy URL:** [https://abhishek04122006.github.io/timezy-privacy-policy/](https://abhishek04122006.github.io/timezy-privacy-policy/)

We will review and respond to inquiries within reasonable and statutory timeframes notified under applicable law. If a grievance under the DPDP Act cannot be resolved through our grievance channel, you may have the option to approach the Data Protection Board of India once that mechanism is formally notified and operative.

---

## 12. Privacy Policy Updates

We may revise this Privacy Policy from time to time to reflect app improvements, Android platform changes, or evolving legal requirements.

When changes are made, we will update the "Last Updated" date at the top of this document. The latest version will always be available in the application repository and within the app distribution. We encourage you to review this policy periodically.
