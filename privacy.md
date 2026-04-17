---
title: Privacy Policy
---

# Privacy Policy

**Last updated:** April 17, 2026

Sweeperbox ("we", "us", "the app") helps you clean your email inbox by swiping through senders. We take your privacy seriously. This policy explains what data we collect, why, and what we do with it.

## TL;DR

- We read your Gmail metadata to identify senders. We **never** read message contents for any purpose other than letting you act on them in the app.
- We **do not sell, rent, share, or use your data for advertising**.
- We **do not** use your Gmail data to train AI/ML models.
- You can revoke our access and delete your account at any time.

## What we collect

When you sign in with Google and grant Gmail access, we collect:

| Data | Why |
|------|-----|
| Email address (from Google) | Identify your account |
| Google user ID | Link your account in our database |
| Sender names + email addresses extracted from your inbox | Show you the list of senders to sweep |
| Per-sender message counts and dates | Sort senders by volume / recency |
| Your Keep / Unsubscribe actions | Update the inbox per your instructions; show history |
| Apple purchase receipts (if you subscribe to Pro) | Verify and unlock Pro features |

We do **not** collect or store:
- Email message bodies
- Email subjects (beyond the brief moment we parse the `From:` header)
- Attachments
- Contact lists
- Your password (Google handles auth — we never see it)

## Gmail API — Limited Use disclosure

Sweeperbox's use of information received from Google APIs adheres to the [Google API Services User Data Policy](https://developers.google.com/terms/api-services-user-data-policy), including the Limited Use requirements.

Specifically:
- We request `gmail.readonly` to identify senders, `gmail.modify` to apply Trash and Important labels when you tap them, and `gmail.settings.basic` to create the unsubscribe filter on your behalf.
- We use Google user data **only** to provide and improve the user-facing features of Sweeperbox.
- We do not transfer Google user data to third parties except as necessary to provide the service (e.g., our infrastructure provider, Supabase) or as required by law.
- We do not use Google user data for serving advertisements, including retargeting, personalized, or interest-based advertising.
- We do not allow humans to read Google user data, except (a) with your explicit consent, (b) for security purposes (e.g., investigating abuse), (c) to comply with applicable law, or (d) where the data has been aggregated and anonymized for internal operations.
- We do not use Google user data to develop, improve, or train generalized AI or machine learning models.

## How we store data

- All data is stored in our Supabase project (PostgreSQL, hosted in the US).
- Authentication tokens (Google OAuth) are encrypted at rest.
- All data in transit uses TLS 1.2 or higher.
- Apple StoreKit receipts are validated against Apple's servers; we store only verification metadata, not the raw receipt.

## Third-party processors

| Processor | Purpose | Data shared |
|-----------|---------|-------------|
| Supabase (database + auth + functions) | Backend storage and processing | All app data |
| Google (Gmail API + Sign-In) | Auth + inbox access | OAuth tokens (we read; Google stores) |
| Apple (StoreKit + App Store Server API) | Subscription management | Receipt verification only |

We have no advertising, analytics, or tracking partners.

## Tracking

We do **not** track you across other apps or websites. We do not use cookies, advertising IDs, or fingerprinting. Apple's privacy nutrition label for our app reflects this — all collected data is "Linked to You, Not Used for Tracking."

## Your rights

- **Revoke Gmail access:** Google Account → Security → Third-party apps → Sweeperbox → Remove access.
- **Delete your account:** Settings → Delete Account in the app. This permanently deletes your profile, all linked accounts, all sender records, and all action history. Best-effort cleanup also removes Gmail filters we created.
- **Export your data:** Email us at nilesh.chrome@gmail.com and we'll send your data in JSON within 30 days.
- **Residents of the EU/UK (GDPR), California (CCPA), and similar jurisdictions** have additional rights to access, correct, port, and delete personal data. Email nilesh.chrome@gmail.com to exercise them.

## Children

Sweeperbox is not directed at children under 13. We do not knowingly collect data from children under 13. If you believe we have, email nilesh.chrome@gmail.com and we will delete it.

## Changes to this policy

We will update the "Last updated" date at the top of this page when material changes are made. For significant changes, we'll notify you in-app on next launch.

## Contact

Questions or concerns:

**Email:** nilesh.chrome@gmail.com
