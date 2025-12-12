# 🚨 HackQuest Bug Report – GitHub Connection Issue

This repository documents a **GitHub Connection Bug** encountered in the **HackQuest Profile Completion Flow**.

A detailed HTML bug report is included in this repository along with screenshots and a video demonstration.  
The bug affects the platform's ability to correctly validate and complete the profile onboarding process when connecting GitHub.

---

## Check live page


---

## 📌 Bug Summary

During the **Complete Profile → Connect GitHub** step:

- The system initially displays **“Connected to GitHub”**
- Immediately after, it switches to an **error message stating GitHub is not connected**
- Despite this error, the **Profile Integrity Score** shows GitHub as **successfully connected**

This contradictory behavior prevents the user from completing the profile setup.

---

## 🧩 Steps to Reproduce

1. Go to your **HackQuest Profile**
2. Click **Complete Profile**
3. Navigate to the **GitHub Connection** step  
4. Click **Connect with GitHub** and authorize
5. Observe:
   - ✔ "Connected to GitHub" (temporary)
   - ❌ When click to continue, error notice that GitHub is not connected
6. Check the **Profile Integrity Score**
   - GitHub appears as **Connected** despite the error state
7. The **Next** button is blocked, preventing profile completion

---

## How to View the Report
To view the full bug report with interactive elements:
1. Open `index.html` in a web browser.
2. The page includes clickable screenshots that open in a fullscreen overlay.
3. The video demonstration is embedded and can be played directly.

## Screenshots
![github-connected](github-connected.png)

![github-connection-error-on-continue](github-connection-error-on-continue.png)

![github-connection-verified1](github-connection-verified1.png)

![github-connection-verified2](github-connection-verified2.png)

---

## Recorded Video Demonstration
The video demonstrates the bug.  
Check the live page to see the video.

