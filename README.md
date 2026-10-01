# LIFE NOVA | लाइफ नोवा | లైఫ్ నోవా

An offline-first health guidance page for Indian families. It tells a person how serious their symptoms may be, what to do now, where to go, and which free schemes apply. Languages: English, हिंदी, తెలుగు, मराठी.

**Not a doctor.** It gives guidance, not a diagnosis. In an emergency call 108 or 112.

## Works without internet
- One self-contained `index.html`. No external fonts, scripts or servers. Nothing is sent anywhere.
- Open it directly from a phone or SD card, or share the file by Bluetooth or WhatsApp.
- When hosted on https (GitHub Pages), `sw.js` caches it so it opens offline after the first visit and can be installed to the home screen.
- Fonts come from the phone. Very old phones may show Telugu or Marathi poorly; test on target devices.

## Host on GitHub Pages
1. Create a repository and upload all files in this folder.
2. Settings > Pages > Deploy from branch > `main` / root.
3. Open the link once with internet; it then works offline.

When you change `index.html`, bump `V` in `sw.js` so phones refresh.

## Coverage
- Districts: all 33 Telangana districts, plus Maharashtra and other sample districts.
- Special needs: mobility, vision, hearing/speech, intellectual or mental health disability, with UDID card information.
- Schemes: Ayushman Bharat PM-JAY, eSanjeevani, Janani Suraksha, Nikshay, Tele-MANAS 14416, ABHA, Aarogyasri (Telangana districts).

## Before real-world use (important)
1. **Facility data is synthetic.** Distances and services are sample values. Replace with a verified directory from the National Health Mission or state health department.
2. **Clinical review.** Have doctors approve the advice and danger signs before public release.
3. **Translations.** Marathi covers the interface, age groups, durations and danger-sign labels; the remaining health tips show in Hindi until a native speaker translates them. Telugu and Hindi were carried over from the original. Have native speakers review all languages. New Telangana and Maharashtra district names are shown in English or transliterated only.
4. **Helplines and scheme rules change.** Verify numbers and eligibility each release.

## Roadmap
Split content into `data/*.json` for community edits; add Kannada, Tamil, Bengali, Odia; add tests for the triage rules; add real ASHA and facility directories per district.

License: MIT
