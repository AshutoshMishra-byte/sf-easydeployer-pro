# Privacy Policy for SF EasyDeployer Pro

**Last Updated:** September 2026

## Overview
SF EasyDeployer Pro ("the Extension") is designed to facilitate the deployment of Salesforce metadata (Custom Objects, Fields, Validation Rules, Permissions) between Salesforce organizations. We are committed to protecting your privacy and ensuring the security of your data.

## Information Collection and Use

### Salesforce Data & Authentication
- **Session Tokens:** The Extension accesses your active Salesforce session (via browser cookies or DOM inspection) strictly to authenticate API requests to your Salesforce org. 
- **Data Transmission:** Your Salesforce session tokens are **never** transmitted to any external servers, third-party services, or Firebase. They remain securely within your local browser environment.
- **Metadata:** The Extension retrieves metadata (e.g., fields, objects, validation rules) from your Source Org to create a deployment package.

### Storage & Firebase Retention
- **Local Storage:** The Extension uses Chrome's `storage.local` API to store your connection details, recent deployment history, and temporary package data to improve performance and enable rollback features.
- **Firebase Realtime Database:** When you generate a 6-character deployment code, the metadata package (containing object structures, field definitions, and validation rules) is temporarily uploaded to our Firebase instance. 
- **Data Retention:** Deployment packages stored in Firebase are strictly temporary and are automatically set to expire and be **deleted after 24 hours**. We do not persistently store, analyze, or sell your Salesforce metadata.

### Cookies
- The Extension requires the `cookies` permission specifically to locate the Salesforce `sid` (Session ID) cookie. This ensures a seamless, no-login-required connection to your currently active Salesforce tab. We do not use cookies for tracking, analytics, or advertising.

## Data Sharing and Disclosure
We do not sell, trade, or otherwise transfer your metadata, deployment packages, or user information to outside parties. All data interactions are strictly between your browser, your Salesforce orgs, and the temporary Firebase transport layer.

## Security
We implement strict Manifest V3 (MV3) security guidelines. The Extension utilizes a secure Content Security Policy (CSP) that restricts external connections solely to verified Salesforce and Firebase endpoints. No inline scripts are executed, mitigating the risk of Cross-Site Scripting (XSS).

## Contact
If you have any questions or concerns regarding this Privacy Policy or the data practices of SF EasyDeployer Pro, please contact Ashutosh Kumar Mishra.
