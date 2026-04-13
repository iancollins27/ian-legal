---
title: Disconnect from QuickBooks Online
---

# Disconnect from QuickBooks Online

This app is a personal, read-only QuickBooks Online connector operated by its
sole owner, Ian Collins. If you need to disconnect or revoke its access to a
QuickBooks Online company, follow the steps below.

## Revoking access via Intuit

1. Sign in to your Intuit account at
   [https://accounts.intuit.com/](https://accounts.intuit.com/)
2. Open **Account Settings** and go to **Apps & Connections**
   (or visit
   [https://qbo.intuit.com/app/connectedapps](https://qbo.intuit.com/app/connectedapps))
3. Locate the app in the list of connected apps
4. Click **Disconnect**

Once disconnected, the stored access token and refresh token are invalidated
by Intuit and the app can no longer read data from the company until a new
authorization is performed.

## Revoking locally

The owner can also revoke access locally by deleting the tokens in
`~/.secrets/quickbooks.secrets` on the machine running the app. This has the
same practical effect on the local machine but does not invalidate the tokens
at Intuit — the disconnect step above is the authoritative revocation.

## Questions

**Ian Collins** — collins.ian27@gmail.com
