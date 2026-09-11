---
title: Meshbar Privacy Policy
layout: default
permalink: /meshbar/privacy/
---

# Meshbar: Tailnet Monitor — Privacy Policy

**Last updated: 11 September 2026**

Meshbar ("the app") is a macOS app developed by Josh Fisk ("we", "us"). This
page describes what data the app handles and where it goes.

## What we collect

**Nothing.** We do not operate any server. Meshbar never sends your tailnet
data, your API key, or any usage data to us or to any third party.

## How the app talks to Tailscale

Meshbar is a client for Tailscale's public API. You create an API access key
in your own Tailscale admin console and paste it into the app. Every request
goes directly from your Mac to `api.tailscale.com` over HTTPS, carrying that
key. The app reads the device list and, if you use the Pro actions, updates a
device's enabled routes or key-expiry setting or removes a device. Those are
the only calls it makes.

Tailscale's handling of that data is governed by
[Tailscale's privacy policy](https://tailscale.com/privacy-policy) and your
organization's agreement with Tailscale.

## What's stored on your Mac

- **Your API access key**, in the macOS Keychain.
- **Device data you look at** is held in memory only while the app is open and
  is not written to disk.
- **Alert preferences and a list of key-expiry alerts already shown**, in the
  app's preferences, so the same expiry isn't reported twice.
- **The date you first launched the app**, in the Keychain, used to compute
  the 7-day trial.

Removing the key in Settings deletes it from the Keychain. Deleting the app
removes its preferences.

## Notifications

If you turn on alerts, Meshbar asks macOS for permission to show
notifications. Notifications are generated on your Mac from the device data
the app has already fetched; nothing is sent to a push service.

## Purchases

Meshbar Pro is sold through Apple's In-App Purchase system. Apple processes
the payment; we never see your payment details. Apple's
[privacy policy](https://www.apple.com/legal/privacy/) applies.

## What we don't use

- Analytics or telemetry
- Advertising networks or identifiers
- Crash-reporting services
- Cookies, web beacons, or tracking
- Third-party SDKs of any kind

## Children's privacy

Meshbar is a tool for network administrators and is not directed at children.
We do not knowingly collect data from anyone.

## Changes to this policy

If the app's data handling ever changes, this page will be updated and the
"Last updated" date revised.

## Contact

[joshfisk3@gmail.com](mailto:joshfisk3@gmail.com)
