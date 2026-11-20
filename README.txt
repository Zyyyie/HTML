Voice Intercom
==============
Files: voice-intercom.html (the app) + sw.js (lets the page open with no internet).
Upload BOTH files to the same folder on dplooy.com (HTTPS is required for the microphone).

ONLINE:  open the page, enter name + channel, everyone on the same channel can talk.
OFFLINE (no internet): put all devices on the same phone hotspot / Wi-Fi.
  1. Open the page once while online beforehand (so it is cached), or open it from the hotspot if it has data.
  2. Tap "Enter intercom" - with no internet it switches to offline mode by itself
     (or tap "No internet? Use offline mode").
  3. One device is the HOST ("Add a person"). Each guest taps "Join a host".
     Guest shows a QR code -> host scans it -> host shows a reply QR -> guest scans it. Repeat per guest.
  4. Everyone taps "Start group call".
QR scanning uses the browser's BarcodeDetector (Chrome on Android). Elsewhere, paste the code text instead.
If the hotspot has "client/AP isolation" turned on, devices cannot see each other.
