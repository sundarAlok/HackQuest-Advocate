# Daily Streak Reward Bug Report

## Webpage Live Link

[See Full Bug Report](https://sundaralok.github.io/HackQuest-Advocate/)

## 🔍 Overview

This repository documents an inconsistency in the **Daily Streak reward system** where the credited points do not consistently match the displayed reward value.

- Displayed Reward: **10 points**
- Actual Reward Observed: **5, 10, 15, 20 (cyclical pattern)**
- Total Streaks Analyzed: **39 days**
- Average Reward: **13.33 points**

The findings indicate a hidden cyclical backend reward logic rather than a fixed reward system.

---

## 📊 Identified Reward Pattern

Observed sequence pattern:

10 → 10 → 15 → 15 → 20 → 20 → 5 → repeat


- If a streak is missed, the sequence resets to **10**
- Distribution over 39 days:
  - 5 pts → 5 times
  - 10 pts → 13 times
  - 15 pts → 11 times
  - 20 pts → 10 times

This contradicts the displayed fixed reward of 10 points.

---

## 🧪 Evidence Included

- Before & After claim screenshots
- 39-day structured data table
- Automatic statistical pie chart visualization
- Screen recording demonstration

---

## 🚀 Live Report

View the full interactive bug report here:

👉 **Live Link:**  
`YOUR_LIVE_LINK_HERE`

---

## ⚙️ Technologies Used

- HTML5
- CSS3 (Modern UI styling)
- JavaScript
- Chart.js (Data visualization)

---

## 📌 Conclusion

The reward system appears to operate on a hidden state-based cycle rather than a constant value as displayed in the UI.

This may indicate:
- Backend logic mismatch
- State tracking issue
- Reward sequence misalignment
- UI/backend desynchronization

---

## 📬 Author

Repository created for analytical bug documentation and structured reporting.
