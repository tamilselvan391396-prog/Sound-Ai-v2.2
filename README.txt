BIOSOUND AI — ANDROID PHONE VERSION

This is a phone-friendly web app, not an APK. It uses Google's pretrained YAMNet audio classifier and MediaPipe Tasks Audio.

IMPORTANT:
1. Live microphone access requires the app to be hosted on an HTTPS website. Opening index.html directly from Downloads will NOT give reliable microphone access.
2. To publish: upload the three files (index.html, manifest.webmanifest, sw.js) to an HTTPS static host such as GitHub Pages or Netlify. Then open the HTTPS address in Chrome.
3. In Chrome, allow microphone permission. Use the browser menu > Add to Home screen / Install app.
4. Internet is needed initially to load the MediaPipe code and YAMNet model. The service worker is a minimal install helper; this first version is not fully offline.

Features:
- Live microphone sound classification
- Top sound label and model score
- Other possible sound labels
- Dominant frequency and live spectrum
- RMS signal level

Limitations:
- YAMNet recognizes broad AudioSet sound classes; it may not distinguish every fan, mixer, refrigerator, bike or car model.
- Scores are not calibrated probabilities.
- Frequency analysis is descriptive, not a separate AI diagnosis.
- Not trained specifically for insects yet.
