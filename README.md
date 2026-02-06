# Ulearn Privacy Policy

**Your privacy matters to us**

*Effective Date: February 6, 2026*

> **Summary:** Ulearn collects only the data necessary to provide its quiz and learning features. Your data is stored securely, never sold to third parties, and you can delete it at any time.

## 1. Introduction

Ulearn ("we", "our", or "the extension") is a Chrome browser extension that generates AI-powered quizzes from YouTube videos to help users learn and retain knowledge. This Privacy Policy explains what data we collect, why we collect it, how we store and protect it, and your rights regarding your data.

By installing and using Ulearn, you agree to the data practices described in this policy.

## 2. Data We Collect

### 2.1 Data You Provide

| Data Type | Purpose |
|-----------|---------|
| Email address | Account creation and authentication via Firebase Auth |
| Display name | Personalization of your dashboard profile |
| Password | Account authentication (stored as a hash by Firebase Auth; Ulearn never has access to your plaintext password) |

### 2.2 Data Collected Automatically

| Data Type | Purpose |
|-----------|---------|
| YouTube video titles and channel names | Generating quizzes and tracking which videos you have studied |
| YouTube video transcript text | Sent to our quiz generation API to create quiz questions. Transcript text is processed in real time and not stored on our servers. |
| Quiz scores and answers | Tracking your learning progress, XP, and achievements |
| Extension usage data (XP, level, coins, achievements) | Powering the gamification and progress-tracking features |
| Avatar customization preferences | Displaying your personalized avatar in the dashboard |

### 2.3 Data We Do NOT Collect

- Your full browsing history (we only detect YouTube video pages)
- Personal files or data from your computer
- Financial information or payment data
- Data from websites other than YouTube
- Cookies or tracking pixels for advertising
- Your YouTube account credentials

## 3. How We Use Your Data

We use the collected data exclusively to:

- **Generate quizzes** from YouTube video transcripts using an AI service
- **Track your learning progress** including videos watched, quiz scores, and streaks
- **Sync your data** across devices via Firebase cloud storage
- **Power gamification features** such as XP, levels, achievements, and the avatar shop
- **Provide daily review quizzes** and final exams based on your learning history

We do not use your data for advertising, profiling, or any purpose unrelated to the extension's learning features.

## 4. Data Storage and Security

### 4.1 Where Your Data Is Stored

- **Locally:** Quiz data, progress, and settings are stored in your browser using Chrome's built-in storage APIs (`chrome.storage.local` and `chrome.storage.sync`).
- **Cloud:** If you create an account, your data is synced to Google Firebase (Firestore database), hosted on Google Cloud Platform infrastructure.

### 4.2 Security Measures

- All data transmitted between the extension and Firebase uses HTTPS encryption (TLS)
- Firebase Authentication handles credential management with industry-standard security
- Firestore Security Rules ensure users can only access their own data
- The extension's Content Security Policy restricts script execution to prevent injection attacks
- Video transcript data is processed in real time by our quiz API and is not permanently stored on our servers

## 5. Third-Party Services

Ulearn uses the following third-party services:

| Service | Purpose | Data Shared |
|---------|---------|-------------|
| Google Firebase (Auth, Firestore) | User authentication and cloud data sync | Email, display name, learning progress |
| Anthropic Claude API (via Cloudflare Worker) | AI-powered quiz generation | Video transcript text (processed in real time, not stored) |

Each third-party service is governed by its own privacy policy:

- [Google Firebase Privacy Policy](https://firebase.google.com/support/privacy)
- [Anthropic Privacy Policy](https://www.anthropic.com/privacy)
- [Cloudflare Privacy Policy](https://www.cloudflare.com/privacypolicy/)

## 6. Data Retention

- **Local data:** Stored in your browser until you uninstall the extension or clear your browser data.
- **Cloud data:** Stored in Firebase as long as your account is active. Data is deleted when you delete your account.
- **Transcript data:** Processed in real time during quiz generation and not retained on our servers after the quiz is created.

## 7. Your Rights

You have the following rights regarding your data:

- **Access:** View all your stored data through the Ulearn dashboard.
- **Portability:** Export your learning progress and resume from the dashboard.
- **Deletion:** Delete your account and all associated cloud data through the dashboard settings. Local data is removed by uninstalling the extension.
- **Opt out of cloud sync:** Use the extension without creating an account. All data will remain local to your browser only.

## 8. Children's Privacy

Ulearn is designed as an educational tool and may be used by learners of all ages. We do not knowingly collect personal information beyond what is described in this policy. If you are a parent or guardian and believe your child has provided personal information without your consent, please contact us so we can take appropriate action.

## 9. Changes to This Policy

We may update this Privacy Policy from time to time. When we make changes, we will update the "Effective Date" at the top of this page. Continued use of the extension after changes are posted constitutes acceptance of the updated policy.

## 10. Permissions Explained

Ulearn requests the following Chrome permissions, each for a specific purpose:

| Permission | Why It's Needed |
|------------|-----------------|
| `activeTab` | To detect when you are on a YouTube video page and read the video information |
| `scripting` | To inject the content script that monitors YouTube videos for quiz generation |
| `storage` | To save your quiz history, progress, and settings locally in the browser |
| `notifications` | To notify you when a quiz is ready or remind you about daily review quizzes |
| `alarms` | To schedule daily review quiz reminders |
| `tabs` | To detect YouTube tab navigation and inject content scripts when needed |

## 11. Contact

If you have questions or concerns about this Privacy Policy or your data, please contact us by opening an issue on our project repository or emailing the developer.

---

*Ulearn -- Privacy Policy -- Last updated February 6, 2026*
