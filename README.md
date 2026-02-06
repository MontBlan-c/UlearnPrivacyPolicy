<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ulearn - Privacy Policy</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.7;
            color: #333;
            background: #f8f9fa;
        }

        .container {
            max-width: 800px;
            margin: 0 auto;
            padding: 40px 24px;
        }

        header {
            text-align: center;
            margin-bottom: 40px;
            padding-bottom: 24px;
            border-bottom: 2px solid #667eea;
        }

        header h1 {
            font-size: 32px;
            color: #667eea;
            margin-bottom: 8px;
        }

        header p.subtitle {
            font-size: 16px;
            color: #666;
        }

        header p.date {
            font-size: 14px;
            color: #999;
            margin-top: 8px;
        }

        h2 {
            font-size: 22px;
            color: #333;
            margin-top: 32px;
            margin-bottom: 12px;
            padding-bottom: 6px;
            border-bottom: 1px solid #e0e0e0;
        }

        h3 {
            font-size: 18px;
            color: #444;
            margin-top: 20px;
            margin-bottom: 8px;
        }

        p {
            margin-bottom: 12px;
        }

        ul {
            margin: 8px 0 16px 24px;
        }

        li {
            margin-bottom: 6px;
        }

        .highlight {
            background: #f0f3ff;
            border-left: 4px solid #667eea;
            padding: 16px 20px;
            margin: 16px 0;
            border-radius: 0 8px 8px 0;
        }

        .highlight p {
            margin-bottom: 0;
        }

        a {
            color: #667eea;
            text-decoration: none;
        }

        a:hover {
            text-decoration: underline;
        }

        footer {
            margin-top: 48px;
            padding-top: 24px;
            border-top: 1px solid #e0e0e0;
            text-align: center;
            color: #999;
            font-size: 14px;
        }

        table {
            width: 100%;
            border-collapse: collapse;
            margin: 16px 0;
        }

        th, td {
            text-align: left;
            padding: 10px 14px;
            border: 1px solid #e0e0e0;
        }

        th {
            background: #f0f3ff;
            color: #333;
            font-weight: 600;
        }

        td {
            background: #fff;
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1>Ulearn Privacy Policy</h1>
            <p class="subtitle">Your privacy matters to us</p>
            <p class="date">Effective Date: February 6, 2026</p>
        </header>

        <div class="highlight">
            <p><strong>Summary:</strong> Ulearn collects only the data necessary to provide its quiz and learning features. Your data is stored securely, never sold to third parties, and you can delete it at any time.</p>
        </div>

        <h2>1. Introduction</h2>
        <p>Ulearn ("we", "our", or "the extension") is a Chrome browser extension that generates AI-powered quizzes from YouTube videos to help users learn and retain knowledge. This Privacy Policy explains what data we collect, why we collect it, how we store and protect it, and your rights regarding your data.</p>
        <p>By installing and using Ulearn, you agree to the data practices described in this policy.</p>

        <h2>2. Data We Collect</h2>

        <h3>2.1 Data You Provide</h3>
        <table>
            <tr>
                <th>Data Type</th>
                <th>Purpose</th>
            </tr>
            <tr>
                <td>Email address</td>
                <td>Account creation and authentication via Firebase Auth</td>
            </tr>
            <tr>
                <td>Display name</td>
                <td>Personalization of your dashboard profile</td>
            </tr>
            <tr>
                <td>Password</td>
                <td>Account authentication (stored as a hash by Firebase Auth; Ulearn never has access to your plaintext password)</td>
            </tr>
        </table>

        <h3>2.2 Data Collected Automatically</h3>
        <table>
            <tr>
                <th>Data Type</th>
                <th>Purpose</th>
            </tr>
            <tr>
                <td>YouTube video titles and channel names</td>
                <td>Generating quizzes and tracking which videos you have studied</td>
            </tr>
            <tr>
                <td>YouTube video transcript text</td>
                <td>Sent to our quiz generation API to create quiz questions. Transcript text is processed in real time and not stored on our servers.</td>
            </tr>
            <tr>
                <td>Quiz scores and answers</td>
                <td>Tracking your learning progress, XP, and achievements</td>
            </tr>
            <tr>
                <td>Extension usage data (XP, level, coins, achievements)</td>
                <td>Powering the gamification and progress-tracking features</td>
            </tr>
            <tr>
                <td>Avatar customization preferences</td>
                <td>Displaying your personalized avatar in the dashboard</td>
            </tr>
        </table>

        <h3>2.3 Data We Do NOT Collect</h3>
        <ul>
            <li>Your full browsing history (we only detect YouTube video pages)</li>
            <li>Personal files or data from your computer</li>
            <li>Financial information or payment data</li>
            <li>Data from websites other than YouTube</li>
            <li>Cookies or tracking pixels for advertising</li>
            <li>Your YouTube account credentials</li>
        </ul>

        <h2>3. How We Use Your Data</h2>
        <p>We use the collected data exclusively to:</p>
        <ul>
            <li><strong>Generate quizzes</strong> from YouTube video transcripts using an AI service</li>
            <li><strong>Track your learning progress</strong> including videos watched, quiz scores, and streaks</li>
            <li><strong>Sync your data</strong> across devices via Firebase cloud storage</li>
            <li><strong>Power gamification features</strong> such as XP, levels, achievements, and the avatar shop</li>
            <li><strong>Provide daily review quizzes</strong> and final exams based on your learning history</li>
        </ul>
        <p>We do not use your data for advertising, profiling, or any purpose unrelated to the extension's learning features.</p>

        <h2>4. Data Storage and Security</h2>

        <h3>4.1 Where Your Data Is Stored</h3>
        <ul>
            <li><strong>Locally:</strong> Quiz data, progress, and settings are stored in your browser using Chrome's built-in storage APIs (<code>chrome.storage.local</code> and <code>chrome.storage.sync</code>).</li>
            <li><strong>Cloud:</strong> If you create an account, your data is synced to Google Firebase (Firestore database), hosted on Google Cloud Platform infrastructure.</li>
        </ul>

        <h3>4.2 Security Measures</h3>
        <ul>
            <li>All data transmitted between the extension and Firebase uses HTTPS encryption (TLS)</li>
            <li>Firebase Authentication handles credential management with industry-standard security</li>
            <li>Firestore Security Rules ensure users can only access their own data</li>
            <li>The extension's Content Security Policy restricts script execution to prevent injection attacks</li>
            <li>Video transcript data is processed in real time by our quiz API and is not permanently stored on our servers</li>
        </ul>

        <h2>5. Third-Party Services</h2>
        <p>Ulearn uses the following third-party services:</p>
        <table>
            <tr>
                <th>Service</th>
                <th>Purpose</th>
                <th>Data Shared</th>
            </tr>
            <tr>
                <td>Google Firebase (Auth, Firestore)</td>
                <td>User authentication and cloud data sync</td>
                <td>Email, display name, learning progress</td>
            </tr>
            <tr>
                <td>Anthropic Claude API (via Cloudflare Worker)</td>
                <td>AI-powered quiz generation</td>
                <td>Video transcript text (processed in real time, not stored)</td>
            </tr>
        </table>
        <p>Each third-party service is governed by its own privacy policy:</p>
        <ul>
            <li><a href="https://firebase.google.com/support/privacy" target="_blank" rel="noopener noreferrer">Google Firebase Privacy Policy</a></li>
            <li><a href="https://www.anthropic.com/privacy" target="_blank" rel="noopener noreferrer">Anthropic Privacy Policy</a></li>
            <li><a href="https://www.cloudflare.com/privacypolicy/" target="_blank" rel="noopener noreferrer">Cloudflare Privacy Policy</a></li>
        </ul>

        <h2>6. Data Retention</h2>
        <ul>
            <li><strong>Local data:</strong> Stored in your browser until you uninstall the extension or clear your browser data.</li>
            <li><strong>Cloud data:</strong> Stored in Firebase as long as your account is active. Data is deleted when you delete your account.</li>
            <li><strong>Transcript data:</strong> Processed in real time during quiz generation and not retained on our servers after the quiz is created.</li>
        </ul>

        <h2>7. Your Rights</h2>
        <p>You have the following rights regarding your data:</p>
        <ul>
            <li><strong>Access:</strong> View all your stored data through the Ulearn dashboard.</li>
            <li><strong>Portability:</strong> Export your learning progress and resume from the dashboard.</li>
            <li><strong>Deletion:</strong> Delete your account and all associated cloud data through the dashboard settings. Local data is removed by uninstalling the extension.</li>
            <li><strong>Opt out of cloud sync:</strong> Use the extension without creating an account. All data will remain local to your browser only.</li>
        </ul>

        <h2>8. Children's Privacy</h2>
        <p>Ulearn is designed as an educational tool and may be used by learners of all ages. We do not knowingly collect personal information beyond what is described in this policy. If you are a parent or guardian and believe your child has provided personal information without your consent, please contact us so we can take appropriate action.</p>

        <h2>9. Changes to This Policy</h2>
        <p>We may update this Privacy Policy from time to time. When we make changes, we will update the "Effective Date" at the top of this page. Continued use of the extension after changes are posted constitutes acceptance of the updated policy.</p>

        <h2>10. Permissions Explained</h2>
        <p>Ulearn requests the following Chrome permissions, each for a specific purpose:</p>
        <table>
            <tr>
                <th>Permission</th>
                <th>Why It's Needed</th>
            </tr>
            <tr>
                <td><code>activeTab</code></td>
                <td>To detect when you are on a YouTube video page and read the video information</td>
            </tr>
            <tr>
                <td><code>scripting</code></td>
                <td>To inject the content script that monitors YouTube videos for quiz generation</td>
            </tr>
            <tr>
                <td><code>storage</code></td>
                <td>To save your quiz history, progress, and settings locally in the browser</td>
            </tr>
            <tr>
                <td><code>notifications</code></td>
                <td>To notify you when a quiz is ready or remind you about daily review quizzes</td>
            </tr>
            <tr>
                <td><code>alarms</code></td>
                <td>To schedule daily review quiz reminders</td>
            </tr>
            <tr>
                <td><code>tabs</code></td>
                <td>To detect YouTube tab navigation and inject content scripts when needed</td>
            </tr>
        </table>

        <h2>11. Contact</h2>
        <p>If you have questions or concerns about this Privacy Policy or your data, please contact us by opening an issue on our project repository or emailing the developer.</p>

        <footer>
            <p>Ulearn &mdash; Privacy Policy &mdash; Last updated February 6, 2026</p>
        </footer>
    </div>
</body>
</html>
