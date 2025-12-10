# Bug Report: Profile HackQuest Score Mismatch

## Project Overview
This project contains a detailed bug report for an issue in the HackQuest platform's user profile page. The bug involves a mismatch in the displayed HackQuest Score statistics, specifically showing incorrect values for "Articles Published" and "Communities Connected" in the summary section compared to the actual detailed sections on the page.

**Reported On:** 10/12/2025  
**Affected Profile:** [HackQuest User Profile](https://www.hackquest.io/user/2087317)

## Bug Description
In the **Profile → HackQuest Score** section, the values are displayed as:
- **Articles Published = 0**
- **Communities Connected = 0**

However, further down on the same profile page:
- The **Article section shows 1 published article**.
- The **Community section shows 2 connected communities**.

This indicates that the HackQuest Score section is not pulling the correct data or not updating properly.

## Criticality & Impact
- **Criticality:** Medium Severity
- **Area of Impact:**
  - UI/Frontend Data Display
  - Backend / Data Fetch Logic

### How This Bug Affects User Experience
- Shows inaccurate HackQuest Score summary.
- Causes confusion for users when comparing the summary vs. detailed sections.
- Reduces trust in profile statistics.
- May affect leaderboard or score-based features if linked.

## Steps to Reproduce (Validate the Bug)
1. Open the user’s Profile page.
2. Scroll to the **HackQuest Score** section.
3. Observe that:
   - Articles Published = 0
   - Communities Connected = 0
4. Now scroll further down to the **Articles section**.
5. You will see **1 article published**.
6. Scroll to the **Communities section**.
7. You will see **2 connected communities**.
8. Mismatch confirmed.

## Files Included
- `index.html`: The main bug report page with detailed description, steps, and embedded media.
- `HackQuest-Score.png`: Screenshot of the HackQuest Score section showing incorrect values.
- `Articles-Published.png`: Screenshot of the Articles section showing 1 published article.
- `Communities-connected.png`: Screenshot of the Communities section showing 2 connected communities.
- `User Profile - HackQuest and 6 more pages - Personal - Microsoft​ Edge 2025-12-10 19-52-45.mp4`: Recorded video demonstration (not included in README for GitHub compatibility).

## How to View the Report
To view the full bug report with interactive elements:
1. Open `index.html` in a web browser.
2. The page includes clickable screenshots that open in a fullscreen overlay.
3. The video demonstration is embedded and can be played directly.

## Screenshots
### HackQuest Score Section (Incorrect Values)
![HackQuest Score](Bugs\India Quack Believers\ProfilePage - HackQuest Score Mismatch/HackQuest-Score.png)

### Articles Section (Correct Value: 1 Article)
![Articles Published](Bugs\India Quack Believers\ProfilePage - HackQuest Score Mismatch/Articles-Published.png)

### Communities Section (Correct Value: 2 Communities)
![Communities Connected](Bugs\India Quack Believers\ProfilePage - HackQuest Score Mismatch/Communities-connected.png)
