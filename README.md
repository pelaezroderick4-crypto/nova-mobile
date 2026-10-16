# NOVA Mobile PWA — Candidate Package

This repository contains the public, installable mobile launcher shell for NOVA Command Center.

## What it does
- Provides a home-screen launcher shell hosted over HTTPS.
- Uses a web app manifest and service worker to support installation and cache the launcher shell only.
- Opens the existing NOVA Command Center deployment; it does not copy operational data or bypass NOVA authentication.

## Important limitations
- This is a launcher, not an offline copy of NOVA. Operational modules require internet access.
- Keep credentials, access tokens, customer records, and other confidential information out of this public repository.
- This repository does not contain NOVA's Apps Script backend.

## Files required at the site root
- `index.html`
- `manifest.webmanifest`
- `service-worker.js`
- `nova-icon.svg`
- `nova-icon-180.png`
- `nova-icon-192.png`
- `nova-icon-512.png`

## Installation
- iPhone/iPad: open the hosted site in Safari, tap Share, then Add to Home Screen.
- Android: open the hosted site in Chrome, open the menu, then choose Install app / Add to Home Screen.

## Deployment note
The Command Center URL configured in `index.html` is the existing deployment supplied for this setup. Test on iPhone Safari and Android Chrome before distributing.
