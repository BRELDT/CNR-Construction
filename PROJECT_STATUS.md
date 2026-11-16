# CNR Construction status

Updated November 16, 2026. The application is in private testing.

## Source and deployment

GitHub Pages publishes from `main` at the repository root. Keep private testing off that publishing source. This branch tracks progress while the recovered application source is retained in the existing hosting project and a verified Git bundle. Use the detailed private handoff to locate the test site, source revision, and deployment configuration.

The application includes Home, Quotes & Invoices, and Jobs, with a standalone PWA build. The test site uses a server-side username-and-password implementation with salted password hashes and expiring sessions. The CNR test database is separate from MAC Industries.

## Verification

- The hosted test build completed. Nine targeted local authentication and backend tests passed.
- The hosted test site blocked signed-out access. The test backend rejected a direct request without server authorization.
- The previous Google-only test app verified all three tabs, quote-to-invoice conversion, recording a payment, expense persistence, routing and fuel costs, projected profitability, and invoice PDF generation. The app recorded test quote and invoice emails as sent. Inbox receipt remains to be confirmed.

## Next steps

1. Complete owner credential setup. Verify hosted sign-in, sign-out, and authenticated access to existing fictional records. Check that the three tabs open and that direct requests without a session are denied.
2. Close enrollment and complete a signed-out browser check before opening public access to the test login.
3. Check the business workflows through the new login and install the PWA on iPhone and Android. Record bugs and results here after each major stage.

Keep CNR test records separate from business records, preserve backups before significant changes, and obtain separate approval for business production use.
