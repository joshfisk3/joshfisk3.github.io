---
title: Postcheck Privacy Policy
layout: default
permalink: /postcheck/privacy/
---

# Postcheck — Privacy Policy

**Last updated: 12 September 2026**

Postcheck is a macOS app developed by Josh Fisk ("we", "us"). This page
describes what data the app handles and where it goes.

## What we collect

**Nothing.** We do not operate any server. Postcheck never sends your domains,
check results, mail, or any usage data to us or to any third party on our
behalf. There is no account, no analytics, no crash reporting and no
advertising.

## What the app sends over the network, and to whom

- **DNS queries** for the domains you add go to Cloudflare (cloudflare-dns.com)
  and, as a fallback, Google (dns.google) over HTTPS. Those providers' privacy
  policies apply to those queries.
- **Blocklist lookups** are DNS queries for your mail servers' addresses against
  public blocklists (Spamhaus, SpamCop, Barracuda, SORBS), sent through the same
  resolvers.
- **Mail server probes** connect to your domain's own mail servers on port 25 to
  test encryption support. No message is sent. This can be turned off in
  Settings.
- **MTA-STS policy files** are fetched over HTTPS from your own domain.
- **Mailboxes you add** are read over IMAP with TLS directly from your mail
  provider to extract DMARC report attachments. Postcheck never modifies or
  deletes mail. If you connect a Gmail account, Postcheck talks to Google's
  OAuth service using an OAuth client you created yourself;
  [Google's privacy policy](https://policies.google.com/privacy) applies.
- **Purchases** are handled by Apple through the App Store.

## What's stored on your Mac

- **Domains, check results, change history and imported DMARC reports**, in
  the app's sandboxed container.
- **Mailbox passwords and Google OAuth tokens**, in the macOS Keychain.
- **Your Google OAuth client ID and preferences**, in the app's preferences.

Removing a mailbox in Settings deletes its Keychain item and revokes the Google
token. Deleting the app removes its container and preferences.

## Purchases

Postcheck Pro is sold through Apple's In-App Purchase system. Apple processes
the payment; we never see your payment details. Apple's
[privacy policy](https://www.apple.com/legal/privacy/) applies.

## What we don't use

- Analytics or telemetry
- Advertising networks or identifiers
- Crash-reporting services
- Cookies, web beacons, or tracking
