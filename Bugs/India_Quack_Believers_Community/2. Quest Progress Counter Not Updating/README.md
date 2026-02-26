# 🐞 Quest Progress Not Updating

## Live page
Click here: [See Full Bug Report](https://sundaralok.github.io/HackQuest-Advocate/Bugs/India_Quack_Believers_Community/2.%20Quest%20Progress%20Counter%20Not%20Updating)

## Overview

This report documents an issue within the **HackQuest – Community Quests module** where quest progress counters fail to update after successfully claiming completed quests.

Although quests display a status of **"Claimed"**, the aggregated progress indicator (e.g., `0/3`, `0/9`) remains unchanged.

---

## Issue Description

When a user completes and claims a quest:

- The quest status updates correctly to **Claimed**
- The progress counter does **not** increment
- The UI continues to display `0/X` progress

This creates a discrepancy between quest status and displayed progress.

---

## Impact

- Inconsistent system state representation
- Reduced user confidence in progress tracking
- Potential logic flaw in aggregation or state synchronization

---

## Reproduction Steps

1. Log in to the platform  
2. Navigate to the Community Quests section  
3. Complete and claim any eligible quest  
4. Observe the progress counter  

---

## Expected Behavior

Progress counters should increment immediately after a quest is successfully claimed.

Example:
```
0/3 → 1/3
```

---

## Actual Behavior

Progress counter remains unchanged:
```
0/3 → 0/3
```

Despite successful completion and claim.

---

## Potential Areas of Investigation

- Backend aggregation logic for completed quests  
- Claim endpoint response payload  
- Frontend state refresh after claim action  
- Caching or delayed synchronization issues  

---

## Supporting Evidence

- Screenshots demonstrating claimed quests with unchanged progress  
- Screen recording showing the issue in real time  

---

## Status

Open – Requires technical review and validation.