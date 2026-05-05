# 🐛 Bug: Quest Reset Freeze (Monthly Reset Not Working)

[![Status](https://img.shields.io/badge/Status-Reported-orange)](https://github.com/)
[![Severity](https://img.shields.io/badge/Severity-High-red)](https://github.com/)
[![Platform](https://img.shields.io/badge/Platform-Web-blue)](https://hackquest.io)
[![Category](https://img.shields.io/badge/Type-State%20Management-purple)](https://hackquest.io)

---

## 📌 Summary
The quest **"Share Your Web3 Learning Journey on Twitter"** does not reset after completion.  
Even after ~1 month (expected cooldown period), the task remains **frozen in "Approved" state** and cannot be attempted again.

---

## 🔄 Reproduce
1. Open `https://www.hackquest.io`
2. Complete the quest and submit required proof (tweet link)
3. Wait for admin approval → ✅ Status becomes **Approved**
4. Wait for reset cycle (~weeks / 1 month)
5. Revisit the quest  

👉 ❌ Quest remains locked / non-resettable

---

## ✅ Expected
- Quest should automatically reset after its cooldown period  
- User should be able to:
  - Reattempt the quest  
  - Submit new proof  
  - Earn points again  

---

## ❌ Actual
- Quest remains permanently in **Approved state**
- No reset triggered
- No retry option available
- UI appears frozen

---

## 🎥 Video Proof
| File | Description |
|------|------------|
| `video.mp4` | Demonstrates quest remains frozen after long duration |

---

## 📸 Screenshots
| Image | Description |
|------|------------|
| `Screenshot (4222).png` | Quest submission page with link |
| `Screenshot (4223).png` | Approved quest still not reset |

---

## 🔍 Root Cause (Suspected)
- Missing or failed backend reset scheduler (cron job)
- Quest lifecycle stuck in "Approved" state
- No state transition to "Available" after cooldown
- Frontend not re-fetching updated quest state

---

## 💡 Fix Suggestions
- Implement/reset scheduler validation (cron job check)
- Add lifecycle transition: `Approved → Reset → Available`
- Add manual fallback reset trigger (admin-side)
- Force client refresh / revalidation of quest state

---

## 🖥️ Environment
- Platform: HackQuest (Web)
- Browser: Chrome / Edge
- OS: Windows

---

## 📎 Attachments
- Screenshots: `Screenshot (4222).png`, `Screenshot (4223).png`
- Video: `video.mp4`
- Optional HTML Report: `bug-report.html`

---

## ⚠️ Impact
This issue breaks the **recurring quest system**, preventing users from:
- Re-engaging with repeatable content  
- Earning additional rewards  
- Maintaining platform activity  

👉 Results in reduced user engagement and trust