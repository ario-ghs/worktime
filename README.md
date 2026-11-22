# Arbeitszeit · Work time

A simple time-tracking app for Android phones, in German and English. It records when you clock in, take breaks, have lunch, return to work and finish the day. At the end of the month it creates an Excel timesheet you can send to your supervisor.

**Open the app:** https://ario-ghs.github.io/worktime/

## Features

- **Clock in / out with one tap:** clock in, start break, start lunch, back to work, finish & go home
- **Daily total:** net working time, time at work and breaks, shown live and when you finish the day
- **Break plan with reminders:** for example 10:00 break (15 min), 12:00 lunch (30 min), 14:00 break (15 min), with a countdown and a "break is over" notice
- **Overtime:** target hours from your contract, daily difference and running overtime balance
- **Absences:** vacation, sick days, time off in lieu, and public holidays for each German state
- **Working Time Act checks (ArbZG):** warnings for short breaks, more than 10 hours a day and less than 11 hours rest
- **Reminders:** "forgot to clock out?" in the evening, a prompt to fix the previous day, and a weekly backup reminder
- **Night shifts:** shifts that run past midnight are counted correctly
- **User profiles:** photo, employee number, position, department, contract type, weekly hours, working days and vacation days; several users on one phone, each with their own data
- **Monthly report:** weekly totals, missing days highlighted, vacation and sick-day counts
- **Excel export:** bilingual German/English timesheet with company logo, employee and contract details, monthly summary, weekly totals and signature fields, set up for printing on A4 landscape
- **PDF timesheet:** the same report as a one-page A4 PDF with logo, summary, weekly totals and signature fields
- **Send to supervisor:** share the PDF directly through email, WhatsApp or any other app. The Excel file is saved to Downloads and can be attached from there
- **Backup and restore:** save all data as a file and load it again, for example on a new phone

## Changelog

- **v1.0:** MIT License added, unused Excel library removed, first official release
- **New address:** repository renamed to `worktime`, app moved to https://ario-ghs.github.io/worktime/
- **PDF sharing:** "Send to supervisor" now shares a PDF timesheet; new "Download PDF" button
- **Profiles and more:** user profiles with photo and contract, overtime, absences and holidays, ArbZG warnings, reminders, weekly totals, night shifts, backup reminder
- **Branding:** GST logo and colors in the app and the Excel file
- **First version:** clock in/out, break plan, daily total, monthly Excel export

## Install on Android

1. Open the link above in **Chrome**.
2. Tap the three-dot menu, then **Install app** (or **Add to Home screen**).
3. Open the app from its icon, create your user and fill in your profile.
4. Tap **Turn on notifications** on the Today screen to get break reminders.

## Your data

All data is stored **only on your phone**. Nothing is sent to a server, and nothing is saved in this repository.

- Data is deleted if you uninstall the app or clear Chrome's site data.
- Save a backup regularly (**Month → Save backup**) and keep your monthly Excel files.

## Limitations

- Notifications work while the app is open or was recently used. Android does not let web apps send scheduled notifications when they are fully closed. For guaranteed reminders, also set alarms in the phone's Clock app.
- Android only lets web apps share certain file types (such as PDF) through the share menu, not Excel files. That is why the app shares a PDF and saves the Excel file to Downloads.
- The Working Time Act warnings are a guide only and are not legal advice.

## Files

| File | Purpose |
|---|---|
| `index.html` | The app |
| `manifest.json` | Makes the app installable |
| `sw.js` | Offline support |
| `xlsx.min.js` | Excel export library ([xlsx-js-style](https://github.com/gitbrent/xlsx-js-style), Apache-2.0) |
| `jspdf.umd.min.js`, `jspdf.plugin.autotable.min.js` | PDF export libraries ([jsPDF](https://github.com/parallax/jsPDF), [jsPDF-AutoTable](https://github.com/simonbengtsson/jsPDF-AutoTable), MIT) |
| `icon-192.png`, `icon-512.png` | App icons |
| `logo.png` | Company logo |

## License

Released under the [MIT License](LICENSE). The GST logo belongs to its owner and is not covered by this license.
