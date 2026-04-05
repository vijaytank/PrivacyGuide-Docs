# Data Safety - Privacy Guide

This document is provided to help you complete the **Data Safety form** in the Google Play Console for Privacy Guide. 

## Data Collection and Security

| Privacy Question                                         | Privacy Guide's Answer                                       |
| -------------------------------------------------------- | ------------------------------------------------------------ |
| Does your app collect or share any user data?            | **No**. We do not collect or share any user data.            |
| Is all user data collected by your app encrypted in transit? | **N/A**. No data is transmitted to an external server.       |
| Do you provide a way for users to request data deletion? | **Yes**. Users can clear all app data via Android Settings. |

## Data Types and Purposes

Although our app processes certain data strictly on the user's device, Google Play's policy requires transparency for any sensitive access. Below is how we handle specific data types:

### 📱 App Inventory (QUERY_ALL_PACKAGES)

- **Data Type**: App inventory/App list.
- **Collection**: No. (Data is accessed for on-device audit and is NOT transmitted).
- **Sharing**: No.
- **Purpose**: App functionality (to audit installed apps for permission risks).

### 🔍 Recent Permission Access (AppOpsManager)

- **Data Type**: Information about how other apps use permissions (Camera, Microphone, etc.).
- **Collection**: No. (Data is logged locally to the device's storage and NOT transmitted).
- **Sharing**: No.
- **Purpose**: App functionality and user education (to provide transparency to the user).

## User Choice and Consent

- **Onboarding Disclosure**: Privacy Guide provides a prominent disclosure during the first launch to explain how and why it processes device information.
- **Opt-in/Opt-out**: Users must explicitly grant necessary permissions and can revoke them at any time.

---

> [!IMPORTANT]
> The `QUERY_ALL_PACKAGES` permission requires a separate **Sensitive Permissions Declaration** in the Play Console. Be sure to justify it as a core requirement for a "Privacy Auditing" tool.
