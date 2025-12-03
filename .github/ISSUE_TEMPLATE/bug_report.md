---
name: 🐞 Bug Report
about: Report a confirmed error, unexpected behavior, or crash within the ScanFlow application.
title: "[BUG] Descriptive summary of the issue"
labels: ["bug", "priority: medium", "status: needs-triage"]
assignees: ['chirag127']
---

As the Apex Technical Authority, we require highly structured and detailed reports to maintain our Zero-Defect philosophy. Please fill out all relevant sections. Incomplete reports may be closed immediately.

### 1. Pre-Check & Verification

*   [ ] I have searched the existing [Issues](https://github.com/chirag127/ScanFlow-CrossPlatform-QRCode-Manager-Mobile-App/issues) to ensure this bug has not already been reported.
*   [ ] I am running the latest available version or the commit hash referenced in the issue body.
*   [ ] This is a reproducible bug, not a configuration or environment setup problem.

---

### 2. Description of the Defect

A concise, high-level summary of the unexpected behavior or crash.

> [Describe the issue clearly and concisely.]

### 3. Steps to Reproduce

**CRITICAL:** Please provide the minimal steps required to reproduce the issue. Include code snippets if necessary, or specify the exact sequence of UI interactions.

1.  Start the `ScanFlow` application on [Specify OS/Device].
2.  Navigate to the [Specific Screen/Feature, e.g., "Scan screen"].
3.  Tap/Interact with [Specific UI Element].
4.  Scan a QR Code of type [e.g., URL, Text, VCard].
5.  Observe the application crash/freeze/unexpected output.

### 4. Expected Behavior

What did you expect the application to do based on the current functionality?

### 5. Actual Behavior

What precisely did the application do instead? If an error message was displayed, include the **full stack trace or error log** within a code block.

typescript
// Paste error logs, stack traces, or device console output here.


### 6. Environment & Technical Details

Providing accurate environment details is paramount for isolating cross-platform defects.

| Component | Detail |
| :--- | :--- |
| **Operating System** | [e.g., iOS 17.5, Android 14] |
| **Device Model** | [e.g., iPhone 15 Pro, Samsung Galaxy S23] |
| **React Native Version** | [Specify RN version] |
| **Expo SDK Version** | [Specify Expo SDK version, e.g., 51.0.0] |
| **`scanflow-core` Library Version** | [Specify version used for scanning logic] |
| **Build Type** | [e.g., Expo Go, Local EAS Build, Installed from Store] |
| **Reproduction Platform** | [e.g., Android Simulator, Physical iOS Device] |

### 7. Supplementary Information

*   If the bug relates to a specific QR Code, please provide an anonymized example or image.
*   Include a short video or GIF demonstrating the issue if possible.
*   Are there any workarounds currently being used?

/cc @chirag127