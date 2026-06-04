# SAML vs OAuth vs OIDC — Quick Reference

| | SAML 2.0 | OAuth 2.0 | OIDC |
|---|----------|-----------|------|
| Purpose | Authentication (SSO) | Authorization (delegated access) | Authentication (built on OAuth) |
| Format | XML assertions | JSON access tokens | JSON ID tokens (JWT) |
| Use case | Workforce SSO (Okta → Salesforce) | "Allow this app to access my Google Drive" | "Sign in with Google" |
| Typical flow | Browser redirect | Authorization code + token exchange | Auth code + ID token |
| Mobile-friendly | Awkward | Designed for it | Yes |
| Era | 2005-ish | 2012 (RFC 6749) | 2014 |
