# 🐞 Bug Report — GitHub Commit Count Mismatch

<br>

## 📌 Overview

This report documents a discrepancy between the commit statistics displayed on the platform dashboard and the actual commit count shown on GitHub's contribution graph.

The issue results in **missing commits being counted**, which affects the accuracy of developer activity metrics.

<br>

# 🌐 Live Report

The full detailed bug report with screenshots and demonstration video can be viewed here:

Live Report: [See Full Bug Report here...](https://sundaralok.github.io/HackQuest-Advocate/)

<br>

# 📊 Report Information

| Field            | Details                                 |
| ---------------- | --------------------------------------- |
| **Report Title** | GitHub Commit Count Mismatch            |
| **Platform**     | HackQuest                               |
| **Severity**     | Medium                                  |
| **Impact**       | Incorrect developer activity statistics |
| **Status**       | Unresolved                              |

<br>

# 🧾 Bug Summary

After connecting a GitHub account with the platform, the commit statistics displayed by the dashboard do **not match the actual commits shown on GitHub**.

### GitHub Contribution Graph

| Year      | Commits         |
| --------- | --------------- |
| **2025**  | 88              |
| **2026**  | 44              |
| **Total** | **132 commits** |

### Platform Dashboard

| Metric            | Value           |
| ----------------- | --------------- |
| Displayed Commits | **119 commits** |

➡️ **13 commits are missing from the platform statistics.**

<br>

# 📷 Evidence Screenshots

### GitHub Contribution Graph (2026)

![GitHub 2026 Commits](Screenshot%20(4168).png)

---

### GitHub Contribution Graph (2025)

![GitHub 2025 Commits](Screenshot%20(4169).png)

---

### Platform Developer Activity

![Platform Commits](Screenshot%20(4170).png)

<br>

# 🎯 Expected Result

The platform should aggregate all GitHub commits correctly and display:

**132 commits**

<br>

# ❗ Actual Result

The platform displays:

**119 commits**

This means **13 commits are not counted by the system.**

<br>

# ⚠️ Possible Root Causes

The discrepancy may be caused by one or more of the following issues:

* GitHub API pagination not implemented correctly
* Only default branch commits counted
* Forked repository commits excluded
* Incorrect time range filtering
* Delayed or cached synchronization of GitHub data

<br>

# 🔁 Steps to Reproduce

1. Login to the platform.
2. Connect your GitHub account.
3. Allow the system to sync GitHub activity.
4. Navigate to **Developer Activity Dashboard**.
5. Compare commit count with the GitHub contribution graph.

<br>

# 🛠 Recommended Fix

To resolve the issue, the following improvements are recommended:

* Verify the GitHub API queries used to fetch commit data.
* Implement proper pagination when fetching commit history.
* Ensure commits from **all repositories** are counted.
* Implement a **manual refresh or scheduled sync mechanism**.

<br>

# 📚 Conclusion

This issue affects the reliability of developer statistics on the platform and may misrepresent user activity.

Correct synchronization with GitHub commit data will ensure accurate developer metrics and improve platform transparency.

<br>

# 📄 License

This report is shared for **security research and responsible disclosure purposes.**
