# 🐞 Bug Report – India Quack Believer “My Quest” Filters

**Reported On:** 2025-12-06

[Open Affected Page](https://www.hackquest.io/my-community/HackQuest/India-Quack-Believers)

---
## Check live page with video
[Live Bug Reporting Page](https://sundaralok.github.io/HackQuest-Advocate/)

## Bug Summary
The **Type Filter** inside the **My Quest** page is not functioning correctly.  
When selecting **Type = Approved**, the system incorrectly shows:

**“Nothing Here”**  

even though approved quests are present and visible without applying the filter.

---

## Criticality & Impact Details

**Criticality:** 🟡 Medium Severity

**Area of Impact:**  
- Frontend / Filtering Logic  
- UI/UX Behavior  

### How This Bug Affects User Experience
- Users cannot filter their quests based on type.  
- Leads to confusion since visible approved items “disappear” when filter is applied.  
- Breaks the core usability of the My Quest page.  
- Makes it difficult for users to track progress or validate rewards.  
- Reduces trust in the filtering system.  

---

## Steps to Reproduce
1. Open the India Quack Believer community homepage.  
2. Click on the **My Quest** button.  
3. Observe that approved quests are visible in the list.  
4. Select any date range using the **Time Range** filter.  
5. Observe that approved quests still remain visible.  
6. Now select **Type = Approved** from the dropdown.  
7. The screen incorrectly shows **“Nothing Here”**.  
8. Repeat with different date ranges or no date range → bug persists.  

---

## Screenshots
Click the images to view larger versions:

| ![My Quest Button](Bugs/my-quest-button.png) | ![Time Range Only](Bugs/time-range-only.png) |
|---------------------------------------|----------------------------------------|
| ![Type Approved](Bugs/type-approved.png)   | ![Type & Time Range Selected](Bugs/type-time-range-selected.png) |

---

## Recorded Video Demonstration
The video demonstrates the bug.  
Check the live page to see the video.
