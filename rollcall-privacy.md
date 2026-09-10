---
title: Rollcall Privacy Policy
layout: default
permalink: /rollcall/privacy/
---

# Rollcall for Google Workspace — Privacy Policy

**Last updated: 9 September 2026**

Rollcall for Google Workspace ("Rollcall") is a macOS app developed by Josh
Fisk ("we", "us"). This page describes what data the app handles and where it
goes.

## What we collect

**Nothing.** We do not operate any server. Rollcall never sends your directory
data, your account information, or any usage data to us or to any third party.

## How the app talks to Google

Rollcall is a client for Google's Admin SDK. When you sign in, the app uses an
OAuth client ID that **you** create in your own Google Cloud project. Every
request goes directly from your Mac to Google's servers over HTTPS, using the
scopes you approve on Google's consent screen:

- `admin.directory.user` — read and update user accounts
- `admin.directory.user.security` — sign a user out of their sessions
- `admin.directory.group.readonly` — list the groups a user belongs to
- `admin.reports.audit.readonly` — reserved for audit-log features; not used in
  the current version

Google's handling of that data is governed by
[Google's privacy policy](https://policies.google.com/privacy) and your
organization's Google Workspace agreement.

## What's stored on your Mac

- **OAuth tokens** for your Google session, in the macOS Keychain.
- **Your OAuth client ID**, in the app's preferences.
- **Directory data you look at** is held in memory only while the app is open
  and is not written to disk.
- **The date you first launched the app**, in the Keychain, used to compute
  the 7-day trial.

Signing out in Settings revokes the Google token and deletes it from the
Keychain. Deleting the app removes its preferences.

## Purchases

Rollcall Pro is sold through Apple's In-App Purchase system. Apple processes
the payment; we never see your payment details. Apple's
[privacy policy](https://www.apple.com/legal/privacy/) applies.

## What we don't use

- Analytics or telemetry
- Advertising networks or identifiers
- Crash-reporting services
- Cookies, web beacons, or tracking
- Third-party SDKs of any kind

## Children's privacy

Rollcall is a business tool for Google Workspace administrators and is not
directed at children. We do not knowingly collect data from anyone.

## Changes to this policy

If the app's data handling ever changes, this page will be updated and the
"Last updated" date revised.

## Contact

[joshfisk3@gmail.com](mailto:joshfisk3@gmail.com)
