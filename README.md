# 🧠 Tes Gaya Kerja (DISC Assessment App)

A web-based psychological assessment tool to measure DISC personality style (Dominance, Influence, Steadiness, Compliance).

---

## 🚀 Tech Stack
- HTML5
- CSS3 (Tailwind CDN)
- Vanilla JavaScript
- Chart.js
- Google Apps Script (for data submission)

---

## 📁 Project Structure

This project is a single-page application structured as follows:

### 1. UI Layer (HTML Sections)
- User Information Form
- Assessment Form (Questions 1–24)
- Results Page

---

### 2. Styling Layer
- Tailwind CSS (utility-based styling)
- Custom CSS:
  - Card animations
  - Button effects
  - Print layout optimization

---

### 3. Data Layer
Contains static assessment data:

- `questions[]`
- `conversionTable`
- `interpretations`

These define:
- Question content
- Scoring logic
- Personality descriptions

---

### 4. State Management
Global variables:
- `currentUser`
- `responses`
- `currentResultData`
- `chartInstances`

---

### 5. Core Logic
Main functions:

#### Assessment Flow
- `startAssessment()`
- `renderQuestions()`
- `handleSelection()`
- `updateProgress()`

#### Scoring System
- `submitAssessment()`
- `determineProfile()`

#### Results Processing
- `getInterpretation()`
- `analyzeGaps()`
- `renderResultsPage()`

---

### 6. External Integration
- Google Apps Script endpoint:
  - Used to store results

---

## 📊 Features

- 24-question DISC assessment
- Dual scoring system:
  - Natural behavior
  - Adapted behavior
- Real-time progress tracking
- Automatic scoring conversion
- Personality profiling logic
- Visualization:
  - Line chart
  - Radar chart
- Print-ready report
- Data submission to Google Sheets

---

## 🧠 DISC Model Explanation

The system evaluates 4 behavior styles:
- D (Dominance)
- I (Influence)
- S (Steadiness)
- C (Compliance)

---

## ⚙️ Future Improvement Ideas

- Split JS into modules
- Move data to JSON file
- Add backend validation
- Add login/session system
- Store results per user
- Improve profiling algorithm
- Add mobile-first optimization

---

## 📌 Notes for Developers

- This is a single-file SPA (no framework)
- All logic runs client-side
- Ensure `conversionTable` remains consistent with question structure
- Avoid modifying `interpretations` keys without updating `determineProfile()`

---

## 📷 Output Example

- Score report per user
- Personality graph visualization
- Comparative Natural vs Adaptation profile

---

## 🛠️ Maintenance Tips

- Keep DATA section separate from logic
- Avoid adding logic inside `submitAssessment()` (refactor recommended)
- Keep UI rendering functions isolated from business logic

---

## 📜 License
Internal / Educational Use
