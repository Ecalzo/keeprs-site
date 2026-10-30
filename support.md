---
title: Keeprs Support
---

# Keeprs Support

Keeprs copies photos from a Ricoh GR IV to your iPhone. This page covers pairing, the things that most often go wrong, and how to report a problem.

## Pairing for the first time

1. On the camera: **Menu › Setup › 6 Communication Settings › Pairing › Execute Pairing**. The camera waits for the phone.
2. In Keeprs, tap **Find camera**. Keep the camera's screen on until every step has a checkmark.
3. Allow Bluetooth and the camera's Wi-Fi when iOS asks. Keeprs stores the camera's Wi-Fi name and password in your Keychain so this only happens once.

After that, opening Keeprs wakes the camera over Bluetooth, joins its Wi-Fi and shows how many photos are new.

## If something goes wrong

Every failure in Keeprs ends in a message that names the step and what to do. The common ones:

- **Camera not found.** Press the camera's power button and keep it awake. If it was never paired with this phone, run Execute Pairing again.
- **Camera does not leave the menu.** Half-press the shutter to return to shooting mode, then tap Retry.
- **iPhone could not join the camera's Wi-Fi.** Tap Open Settings and join the network named `GR_…` by hand, then come back to Keeprs. The password is under the camera's Communication Settings.
- **Camera stopped responding mid-import.** The GR IV drops its Wi-Fi about a minute into the first session. Keeprs reconnects and resumes on its own; anything that did not make it stays selected so a retry is one tap.
- **Slow imports.** The GR IV's Wi-Fi is 2.4 GHz only. Originals arrive at roughly half a megabyte per second; choose **Small JPEGs** on the home screen for 1920 px files that take a few seconds each. DNG files are always saved in full.
- **Keeprs cannot see my old photos.** By design. Keeprs asks for add-only Photos access and never reads your library. Imported photos appear in the Photos app's Recents.

## Diagnostics

Keeprs keeps a short log of connection and import events on your phone. Open **Settings (gear icon) › Diagnostics** to read it and use the share button to send it along with a report. Wi-Fi passwords are redacted from the log.

## Reporting a problem

Open an issue at [github.com/Ecalzo/GRIV-ios/issues](https://github.com/Ecalzo/GRIV-ios/issues) with the camera's firmware version, the iOS version, what you expected, what happened, and the diagnostics log if you have it.

## Privacy

Keeprs has no account, no servers and no analytics. The full policy is on the [privacy page](privacy).

Keeprs is an independent app and is not affiliated with or endorsed by Ricoh. RICOH and GR are trademarks of Ricoh Company, Ltd.
