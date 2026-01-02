# 🚨 HackQuest Bug Report – Temporary Email Detection Failure

This repository documents a **Temporary / Disposable Email Bypass Bug** in the **HackQuest User Registration & Onboarding Flow**.

A detailed **HTML bug report** is included along with screenshots and (optional) video evidence.  
The issue allows users to successfully register and become active platform users using **temporary email services**, which the system fails to detect or block.

<br>

## 🔗 Check Live Page
[Live Bug Report](https://sundaralok.github.io/HackQuest-Advocate/)

<br>

## 📌 Bug Summary

During the **user signup and onboarding process** on HackQuest:

- Users can register using **temporary / disposable email addresses**
- The system does **not flag, restrict, or block** these email domains
- The account becomes a **fully functional HackQuest user**
- No validation error or warning is shown

This allows the creation of **throwaway or fake accounts**, weakening platform trust and security.

<br>

## 🧩 Steps to Reproduce

1. Open any **temporary / disposable email service**
2. Copy the generated temp email address
3. Go to **HackQuest Signup**
4. Register using the temporary email
5. Complete email verification
6. Finish onboarding
7. Observe:
   - ✔ Account is successfully created
   - ✔ Full dashboard access is granted
   - ❌ No restriction or detection of temp email usage

<br>

## ⚠️ Impact & Risk

- Enables creation of **multiple fake accounts**
- Can be abused for:
  - Reward farming
  - Referral manipulation
  - Spam or malicious activity
- Reduces **user authenticity and platform credibility**
- Weakens onboarding and trust validation mechanisms

<br>

## 🧪 How to View the Report

To view the complete interactive bug report:

1. Open `index.html` in a web browser  
2. The page includes:
   - Clickable screenshots with fullscreen preview
   - Clear bug explanation and impact analysis
3. (If included) The video demonstration can be played directly on the page

<br>

## 🖼️ Screenshots

![Before SignUp](Screenshot(3750).png)

![Afetr Using Temp Mail](Screenshot(3751).png)

<br>

## 🎥 Recorded Video Demonstration

A recorded video demonstrates the full bypass flow using a temporary email.  
Please check the **live page** to view the embedded video proof.

---

## 🛠️ Suggested Fix (High-Level)

- Block known disposable email domains
- Integrate a temporary email detection API
- Add server-side validation during signup
- Prevent reward/referral eligibility for unverified email domains

---

**Severity:** High  
**Category:** Security / Authentication / Trust Validation
