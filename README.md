<div align="center">

# 🏋️ MacroTracker AI

**Snap a photo of your meal. Get calories and macros in seconds.**

A single-file, installable web app for tracking calories and protein, with an underwater theme, glassmorphism UI and AI food recognition.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)
![GSAP](https://img.shields.io/badge/GSAP-88CE02?logo=greensock&logoColor=black)
![Gemini](https://img.shields.io/badge/Google%20Gemini-4285F4?logo=googlegemini&logoColor=white)

</div>

---

## ✨ Features

- 📸 **AI food scanning**: take or upload a photo and Google Gemini estimates the food name, calories, protein, carbs and fat.
- 🎯 **Personalised goals**: an onboarding flow takes your profile and goal (lose weight, maintain or gain muscle) and works out daily calorie and protein targets.
- 📊 **Live gauges**: calorie and protein dials fill as you log, and show when you reach or go over your target.
- 🥣 **Today's Log**: frosted-glass food cards with a thumbnail and macro chips. Tap a card for details, or use the menu to edit or delete.
- 🗑️ **Delight in the details**: deleting a meal sucks it into a little bin, genie-style, with a cute sound.
- 🌊 **Immersive intro**: an animated dive from the sky into the ocean, built with GSAP.
- 🫧 **Living background**: dumbbell-in-bubble shapes drift up the screen behind the app.
- 📱 **Installable and mobile-first**: designed for phones, with safe-area support and an "Add to Home Screen" icon.
- 🔒 **Private by design**: no account and no backend. Your data stays in your browser's `localStorage`.

## 🧰 Tech stack

| Area | Choice |
| --- | --- |
| App | One `index.html`: plain HTML, CSS and JavaScript, no build step |
| Animation | [GSAP](https://gsap.com/) for the intro, Web Animations API for UI motion |
| Audio | Web Audio API, with generated sounds and no audio files |
| AI | Google Gemini (`gemini-2.5-flash`) vision API |
| Storage | Browser `localStorage` |

## 🚀 Getting started

1. **Clone the repo**
   ```bash
   git clone https://github.com/Danialbroz/macro-tracker.git
   cd macro-tracker
   ```
2. **Open it**: open `index.html` in a browser, or serve the folder with any static server:
   ```bash
   npx serve .
   ```
3. **Add your Gemini API key**: get a free key from [Google AI Studio](https://aistudio.google.com/apikey), then open the app's settings (⚙️) and paste it in. The key is stored only on your device.

> The intro loads GSAP from a CDN, so you need an internet connection on first load.

## 📖 How to use

1. Complete the short onboarding to set your goal.
2. Tap the scan button, take a photo of your meal, and confirm the result.
3. Watch your gauges fill through the day.
4. Edit or delete entries from the ⋮ menu on any card.

## 🔐 Privacy and security note

All data lives in your browser. Photos you scan are sent directly from your device to Google's Gemini API, and your API key is kept in `localStorage`. Don't share a device or browser profile that holds a key you care about, and use a key restricted to the Generative Language API.

## 🗺️ Roadmap

- [ ] Weekly and monthly history view
- [ ] Manual food search and barcode scanning
- [ ] Export your data

## 🤝 Contributing

Ideas and pull requests are welcome. Open an issue first to discuss larger changes.

## 👤 Author

**Muhammad Danial bin Zainal Abiddin**: [@Danialbroz](https://github.com/Danialbroz)

---

<div align="center">

Made with 💙 and a lot of bubbles.

</div>
