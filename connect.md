---
title: Connect to QuickBooks Online
---

# Connect to QuickBooks Online

This app is a personal, read-only QuickBooks Online connector operated by its
sole owner, Ian Collins, on his own machine against his own QuickBooks
company. It is not distributed to third parties and is not offered as a
service.

## How authorization works

Because the app runs locally and has no hosted web interface, there is no
web-based "Connect" button. Authorization happens from the owner's terminal:

1. The owner runs the `auth` script included in the connector source
2. The script spins up a local HTTP listener on `http://localhost:8080/callback`
3. A browser opens to Intuit's consent page
4. The owner signs in and approves the connection to their own QuickBooks
   company
5. Intuit redirects back to `localhost`, and the script exchanges the
   authorization code for access and refresh tokens
6. Tokens are saved locally with owner-only file permissions and auto-refresh
   on use

## Reconnecting

If the refresh token expires or is revoked, the owner re-runs the same `auth`
script to re-authorize. No action is required from anyone other than the
owner.

## Questions

**Ian Collins** — collins.ian27@gmail.com
