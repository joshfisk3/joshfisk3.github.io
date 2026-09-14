---
title: Shoreline Privacy Policy
layout: default
permalink: /shoreline/privacy/
---

# Shoreline Privacy Policy

**Last updated: 14 September 2026**

Shoreline is a macOS menu-bar app for DigitalOcean developed by Josh Fisk
("we", "us"). This page describes what data the app handles and where it goes.

## What we collect

**Nothing.** Shoreline has no server, no account system and no analytics. We
never receive any data from your copy of the app.

## What the app does with your data

- **DigitalOcean personal access token.** You paste it into the app. It is
  stored in your macOS Keychain and sent only to `api.digitalocean.com`, as
  the Authorization header on requests the app makes on your behalf (droplets,
  apps, databases, load balancers, volumes, domains, firewalls, projects,
  billing, monitoring, and the droplet actions you confirm).
- **SSH key or password (optional).** If you set one up for the pm2 panel or
  the in-app terminal, it is stored in the Keychain and used only to open an
  SSH connection from your Mac directly to your droplet's IP address. Host
  keys are trusted on first use and pinned afterwards.
- **DigitalOcean status.** Every five minutes the app fetches
  `status.digitalocean.com/api/v2/status.json` without any credentials, to
  show an incident banner.
- **Settings.** Alert preferences, muted droplets and known host keys are
  stored locally in the app's preferences.

Nothing is sent anywhere other than DigitalOcean's API, DigitalOcean's status
page, and your own droplets over SSH.

## Purchases

Shoreline Pro is a one-time in-app purchase processed by Apple. We don't
receive your payment details.

## Removing your data

Delete the account in **Settings → Accounts** to remove the token and SSH
credential from the Keychain, and revoke the token in your DigitalOcean
account. Deleting the app removes its preferences.

## Contact

[joshfisk3@gmail.com](mailto:joshfisk3@gmail.com)
