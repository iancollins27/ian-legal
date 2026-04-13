# Privacy Policy

**Last updated:** April 13, 2026

This Privacy Policy describes how personal software tools owned and operated by
Ian Collins ("we", "our", "the Software") handle information when connecting to
third-party services such as QuickBooks Online on behalf of the sole user and
owner.

## Scope

The Software is a personal, locally-run integration. It is operated by and
used solely by its owner, Ian Collins, against accounts owned by Ian Collins.
It is not distributed to third parties and is not offered as a service to
other users.

## Information We Access

When authorized via OAuth, the Software may access read-only data from
connected services, including but not limited to:

- **QuickBooks Online:** company information, chart of accounts, transactions
  (invoices, bills, payments, journal entries, etc.), customers, vendors, items,
  and financial reports (profit and loss, balance sheet, cash flow, aged
  receivables, aged payables, and similar)

The Software is strictly **read-only**: it never creates, updates, or deletes
any record in any connected service.

## How We Use Information

Accessed data is used exclusively for the owner's own analysis, reporting,
and decision-making. Data is processed locally on the owner's machine. No
accessed data is shared with, sold to, or otherwise transmitted to any third
party other than the upstream service it originated from (e.g. QuickBooks
Online).

## Storage and Retention

- **OAuth tokens** (access tokens, refresh tokens, realm identifiers) are
  stored locally on the owner's machine in a protected secrets file with
  owner-only file permissions. They are never transmitted to any party other
  than the upstream service's token endpoint for the purpose of refreshing
  access.
- **Query responses** are processed in memory by the Software and are not
  persisted to disk by default. Any analysis notes or derived summaries the
  owner chooses to save are kept locally on the owner's machine.
- No analytics, telemetry, crash reporting, or usage tracking is performed.

## Third-Party Sharing

We do not share, sell, rent, or disclose any accessed information to any third
party. The Software makes no outbound network requests other than:

1. The upstream service's API (e.g. QuickBooks Online) to retrieve data
2. The upstream service's OAuth token endpoint to refresh credentials

## User Rights and Revocation

As the sole user and owner of the Software, the owner may revoke access at
any time by:

- Disconnecting the Software from the upstream service via that service's
  connected-apps dashboard (for QuickBooks Online: Intuit Account Settings →
  Apps & Connections)
- Deleting the local secrets file containing stored OAuth tokens

## Security

OAuth credentials are stored with restrictive file permissions (mode 0600 on
POSIX systems). The Software is not network-exposed: it runs as a local
process communicating with Claude Code over standard input and output.

## Changes to This Policy

This policy may be updated from time to time. Updates will be reflected in
the "Last updated" date above and committed to the public repository at
`github.com/iancollins27/ian-legal`.

## Contact

Questions or concerns may be directed to:

**Ian Collins**
Email: collins.ian27@gmail.com
