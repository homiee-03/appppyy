# Skywalkers SSC CGL 2026 Test Series

Production-ready SSC CGL Tier-1 test series web app with 50 free tests, custom timers, instant scoring, and Firebase authentication. Fully static and compatible with GitHub Pages.

## ✅ Features
- 50 full-length Tier-1 tests (Test 1 → Test 50)
- Custom timer selection: 60 / 75 / 90 minutes
- SSC standard marking scheme (+2, -0.50, 0)
- Testbook-style dashboard (attempted tests, best score, accuracy)
- Best-score storage per user & per test
- JSON-based question system (`/data` folder)
- Mobile-first blue & white UI

## 📁 Folder Structure
```
.
├── index.html
├── styles.css
├── data/
│   ├── test-1.json
│   ├── test-2.json
│   └── ... test-50.json
```

## 🧾 How to Upload Questions
1. Go to `/data` folder.
2. Replace the contents of any `test-<number>.json` file with your own questions.
3. Use the JSON format below:
```json
{
  "question": "",
  "options": ["A", "B", "C", "D"],
  "correct": 2,
  "explanation": ""
}
```
4. Make sure each test file is an **array** of questions.

## ➕ How to Add More Tests
1. Create a new JSON file in `/data` named `test-51.json`, `test-52.json`, etc.
2. Update the `TEST_COUNT` constant in `index.html` to the new total.

## 🚀 Deploy on GitHub Pages
1. Push this repository to GitHub.
2. Go to **Settings → Pages**.
3. Choose branch `main` (or `work`) and `/root` directory.
4. Save and visit your provided GitHub Pages URL.

## 🔐 Firebase Auth
The Firebase authentication config is already integrated in `index.html`. Do not modify the config or auth logic unless you are replacing it with your own Firebase project.
