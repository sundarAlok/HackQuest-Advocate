# 🐛 Bug: "Get Daily Treasure" Client Error

[![Status](https://img.shields.io/badge/Status-Reported-orange)](https://github.com/sundarAlok/HackQuest-Advocate)
[![Severity](https://img.shields.io/badge/Severity-Medium-yellow)](https://github.com/sundarAlok/HackQuest-Advocate)
[![Platform](https://img.shields.io/badge/Platform-Web-blue)](https://hackquest.io)
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)

## 📌 Summary
"Get Daily Treasure" button throws generic client-side error after completing all 3 daily tasks (streak claim + 4 likes + 1 unit).

## 🔄 Reproduce
1. Go to `hackquest.io` home page
2. Claim daily streak points
3. Like 4 projects
4. Finish 1 learning unit
5. Click "Get Daily Treasure" button
6. ❌ Error: `Application error: a client side error has occurred`

## ✅ Expected
Reward claimed successfully with confirmation.

## ❌ Actual
Generic error modal; console shows no useful debug info.

## 🎥 Videos
| Video | Purpose |
|-------|---------|
| `vid1.mp4` | Full reproduction flow |
| `vid2.mp4` | Another video |

## 🔍 Root Cause (Suspected)
- Unhandled API error / missing try-catch
- Silent backend failure (5xx/malformed response)
- Auth token or state sync issue

## 💡 Fix Suggestions
- Add structured error handling + user-friendly messages
- Implement client-side pre-validation of reward conditions

## 🖥️ Env
`Chrome/Firefox/Edge` | `Windows/macOS/Linux` | `hackquest.io` (Prod)

## 📎 Attachments
- [bug-report.html](https://sundaralok.github.io/HackQuest-Advocate/Bugs/HackQuest_Platform/Get%20Daily%20Treasure/) — Interactive report page
- Videos: `vid1.mp4`, `vid2.mp4`