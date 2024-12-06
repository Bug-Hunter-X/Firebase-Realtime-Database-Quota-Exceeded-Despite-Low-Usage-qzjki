# Firebase Realtime Database Quota Exceeded Bug

This repository demonstrates a common, yet difficult-to-diagnose bug in Firebase's Realtime Database: exceeding the quota despite seemingly low usage.  The bug is rooted in unintentional repeated data writes, often hidden within event listeners or loops.  The provided code examples showcase the issue and its resolution.

**Bug:**  `quotaExceededBug.js` demonstrates a function that unnecessarily updates data, quickly exceeding the write quota.

**Solution:** `quotaExceededSolution.js` provides a corrected version, using techniques to prevent redundant writes.