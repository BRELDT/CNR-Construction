# CNR Construction status

Updated November 16, 2026. The application is in private testing.

## Source and deployment

GitHub Pages publishes from `main` at the repository root. Keep private testing off that publishing source. This branch tracks progress while the recovered application source is retained in the existing hosting project and a verified Git bundle. Use the detailed private handoff to locate the test site, source revision, and deployment configuration.

The application includes Home, Quotes & Invoices, and Jobs, with a standalone PWA build. The test site uses a server-side username-and-password implementation with salted password hashes and expiring sessions. The CNR test database is separate from MAC Industries.

## Verification

- The hosted test build completed.
- The hosted test site blocked signed-out access. The test backend rejected a direct request without server authorization.
- The previous Google-only test app verified all three tabs, quote-to-invoice conversion, recording a payment, expense persistence, routing and fuel costs, projected profitability, and invoice PDF generation. The app recorded test quote and invoice emails as sent. Inbox receipt remains to be confirmed.

## Safari repair

Fixed and redeployed the existing private test site. Verified the styled dashboard, existing records, sign-in, sign-out, all three tabs at desktop and mobile widths, and denial of direct API access without a session. Twelve automated tests and the local Chromium workflow passed.

## Next steps

Keep the app in private testing. Before a future public test, disable enrollment and repeat the signed-out checks. Complete physical-device PWA testing and verify the remaining business workflows using fictional records. Update this file after major stages and obtain separate approval before business production use.
