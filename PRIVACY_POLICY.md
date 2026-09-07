# 🔒 Privacy Policy for SF EasyDeployer Pro

**Last Updated:** September 2026  
**Developer:** Ashutosh Kumar Mishra  
**Product:** SF EasyDeployer Pro (Chrome Extension)

---

## 🛡️ Overview

SF EasyDeployer Pro ("the Extension") helps Salesforce Admins and Developers deploy metadata (Custom Objects, Fields, Validation Rules, and Permissions) between Salesforce orgs using a simple 6-character code.

We are committed to protecting your privacy and handling data with transparency and care. This policy explains what we access, how we use it, and what we never do.

---

## 📥 Information We Access

### 🔐 Salesforce Authentication
- **Session Tokens (`sid` cookie):**  
  The Extension reads your active Salesforce session from browser cookies (or via a secure DOM fallback) **only** to authenticate API requests to **your own** Salesforce org.
- **Important:** Your Salesforce session tokens are **never** sent to Firebase, our servers, or any third party. They stay inside your local browser environment.

### 📦 Salesforce Metadata
- The Extension retrieves **metadata only**, such as:
  - Custom Object definitions  
  - Custom Field definitions  
  - Validation Rules  
  - Global Value Sets  
  - Profile names (for FLS assignment)
- ❌ We do **not** access, read, or transmit customer business records (Accounts, Contacts, Opportunities, Leads, Cases, etc.).

---

## 💾 Storage & Data Retention

### 🖥️ Local Browser Storage
We use Chrome’s `storage.local` API to save:
- Connection details (instance URL, user info)
- Deployment history (last 50 deployments)
- Temporary package data for rollback

This data never leaves your device unless you explicitly generate a shareable deployment code.

### ☁️ Firebase Realtime Database (Temporary Bridge)
When you click **Generate Code**:
- A metadata package is temporarily uploaded to Firebase Realtime Database
- This enables sharing between orgs via a 6-character code (e.g., `SF-A1B2C3`)
- **Retention:** Packages automatically expire and are **deleted after 24 hours**
- We do not permanently store, mine, analyze, or sell your metadata

### 🍪 Cookies
- Permission used **only** to read the Salesforce `sid` session cookie
- ❌ No tracking cookies  
- ❌ No advertising cookies  
- ❌ No analytics cookies  

---

## 🚫 What We Do NOT Collect

| Data Type                        | Collected? |
|----------------------------------|------------|
| Passwords / Login credentials    | ❌ No      |
| Customer / Business records      | ❌ No      |
| Personal identity documents      | ❌ No      |
| Browsing history outside SF      | ❌ No      |
| Location data                    | ❌ No      |
| Analytics / Advertising data     | ❌ No      |
| Financial or health information  | ❌ No      |

---

## 🔗 Data Sharing & Third Parties

We do **not** sell, rent, trade, or share your data for marketing or advertising.

The only external service used is:

- **Google Firebase Realtime Database** — temporary storage of deployment packages (auto-deleted after 24 hours)

All other communication is directly between:
- Your browser  
- Your Salesforce orgs  
- Firebase (temporary transport only)

---

## 🧱 Security Practices

SF EasyDeployer Pro is built with modern security standards:

- ✅ **Manifest V3** compliant  
- ✅ Strict **Content Security Policy (CSP)**  
- ✅ No remote code execution  
- ✅ No `eval()` or inline scripts  
- ✅ HTTPS-only network requests  
- ✅ Minimum required permissions only  
- ✅ Host permissions limited to Salesforce + Firebase domains  

---

## 👤 Your Choices & Control

You can:
- Clear deployment history anytime from the Extension’s History tab  
- Remove the Extension to delete all local data  
- Avoid generating a code if you don’t want metadata uploaded to Firebase  
- Use the **Download Package File** option to share packages offline without Firebase  

---

## 📬 Contact

If you have questions about this Privacy Policy or our data practices, contact:

**Ashutosh Kumar Mishra**  
📧 Email: `ashutoshmishra6033@gmail.com`  
🌐 Chrome Web Store: SF EasyDeployer Pro  

We will respond to privacy-related requests as quickly as possible.

---

## 🔄 Changes to This Policy

We may update this Privacy Policy from time to time.  
The latest version will always be available at this URL and reflected in the Chrome Web Store listing.

**Last Updated:** September 2026

---

*Built with ❤️ for Salesforce Admins & Developers*
