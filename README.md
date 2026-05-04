# HackQuest Bug Report
> Progress Display Discrepancy — Profile Overview vs Learning Progress

[![Status](https://img.shields.io/badge/Status-Reported-orange)](https://github.com/sundarAlok/HackQuest-Advocate)
[![Severity](https://img.shields.io/badge/Severity-Medium-yellow)](https://github.com/sundarAlok/HackQuest-Advocate)
[![Platform](https://img.shields.io/badge/Platform-Web-blue)](https://hackquest.io)

---

## 🐛 Bug Summary

**Title:** Inconsistent Course Completion Status Display  
**Reported:** April 25, 2026  
**Affected Component:** Profile Overview / Learning Progress Module

The **Profile Overview** section displays incorrect progress indicators for completed courses, showing them as partially completed even when the **Learning Progress** page confirms 100% completion with issued certificates.

| Attribute | Details |
|-----------|---------|
| **Severity** | Medium |
| **Impact** | User Experience, Engagement, Trust |
| **Reproducibility** | Consistent |
| **Environment** | Web (Chrome/Edge, Windows) |

---

## 🔄 Steps to Reproduce

1. Navigate to your HackQuest profile: `hackquest.io/user/<your_id>`
2. Open the **Overview** tab and locate the *Learning Progress* section
3. Note the progress bars for completed courses (e.g., Ethereum, Arbitrum)
4. Navigate to **Learning Progress** page: `hackquest.io/learning-progress`
5. Compare completion status between both views
6. **Observed:** Courses marked "Completed ✓" in Learning Progress show partial progress in Overview

---

## 📸 Evidence

Visual proof is included in the interactive report:

| File | Description |
|------|-------------|
| `bug-report.html` | Self-contained interactive report with gallery & video |
| `screenshot1-overview.png` | Profile Overview showing incorrect progress |
| `screenshot2-portfolio.png` | Portfolio with completed certificates |
| `screenshot3-learning-progress.png` | Learning Progress showing completed status |
| `bug-demonstration.mp4` | Screen recording of the discrepancy |

> 💡 Open [index.html](https://sundaralok.github.io/HackQuest-Advocate/) in a browser to view the full interactive report with clickable image lightbox and embedded video.

---

## 🔍 Potential Root Causes

- Data synchronization delay between modules
- Different API endpoints returning inconsistent progress data
- Client-side caching serving stale progress information
- Divergent progress calculation logic across components
- Missing real-time state propagation after course completion

---

## 💡 Recommended Actions

1. **Unify data source** for progress display across all views
2. **Implement cache invalidation** upon course completion events
3. **Audit progress calculation logic** for consistency
4. **Add visual completion indicators** (badges/checkmarks) alongside progress bars
5. **Introduce real-time sync** (WebSocket/polling) for cross-component updates

---

## 🚀 How to View This Report

1. Clone or download the repository
```bash
git clone https://github.com/sundarAlok/HackQuest-Advocate.git
```
2. Navigate to the report directory
```bash
cd HackQuest/bug-report
```

3. Open the interactive report in your browser
```bash
open bug-report.html          # macOS
start bug-report.html         # Windows
xdg-open bug-report.html      # Linux
```

> No dependencies required. The report is a standalone HTML file with embedded CSS/JS.

---

##  Contributing

Found additional issues or have suggestions?

1. Fork the repository
2. Create a feature branch: `git checkout -b fix/progress-sync`
3. Commit your changes: `git commit -m "Add progress sync fix"`
4. Push to the branch: `git push origin fix/progress-sync`
5. Open a Pull Request with detailed description

---

## 📄 License

This bug report is submitted for the purpose of improving the HackQuest platform.  
© 2026 HackQuest Community Feedback Initiative
