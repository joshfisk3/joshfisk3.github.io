---
title: Postcheck
layout: default
permalink: /postcheck/
---

# Postcheck

**Email authentication health for your domains, from your Mac's menu bar.**

Postcheck checks MX, SPF, DKIM, DMARC, MTA-STS, TLS-RPT and BIMI for every
domain you add, looks up your mail servers on the major blocklists, grades the
domain A–F, and tells you in plain English what is wrong and the exact DNS
record that fixes it. Built for IT admins, MSPs and small businesses whose mail
is landing in spam.

- Every finding comes with the host, type and value to publish
- SPF flattener for records over the 10-lookup limit, with drift reminders
- Provider wizards for Google Workspace, Microsoft 365, HubSpot, Mailchimp,
  SendGrid, QuickBooks and Zendesk, compared with live DNS
- Re-checks every six hours, notifies on changes, keeps a timeline of every
  record change
- Reads DMARC aggregate reports from your mailbox, dropped files or a watched
  folder and tells you whether it is safe to move to quarantine or reject
- PDF and Markdown reports; one branded PDF for all of a client's domains
- DNS over HTTPS only; nothing is sent to any server of ours
- Free: one domain, manual checks, grade and fixes. Postcheck Pro is a
  one-time purchase. No subscription.

## Common questions

**Port 25 shows "inconclusive".** Most home and office networks block outbound
port 25. The probe is optional and can be turned off in Settings.

**Spamhaus shows "could not be queried".** Spamhaus refuses lookups relayed
through public DNS resolvers, which is how Postcheck resolves names. Check the
address at spamhaus.org.

**My DKIM key is not found.** Add your provider's selector via the key icon in
the toolbar. Amazon SES, Postmark, SendGrid and HubSpot generate per-account
selectors that cannot be guessed.

**Reports never arrive in my mailbox.** Reports go to the address in your DMARC
record's `rua=`. If that address is at a different domain, that domain must
publish an authorisation record; Postcheck flags this.

**Gmail as a report mailbox.** Postcheck signs in with an OAuth client you
create in your own Google Cloud project; the guide is in Settings → Report
Sources and in the README.

## Support

- Email: [joshfisk3@gmail.com](mailto:joshfisk3@gmail.com)
- [Privacy policy](/postcheck/privacy/)

Please include the domain and, if you can, the Export → Markdown output for it;
it contains everything Postcheck saw.
