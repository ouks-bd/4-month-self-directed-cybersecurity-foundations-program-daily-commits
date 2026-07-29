# Diagrams

## Target weekend diagram
Draw the OIDC "Sign in with Google" flow:
1. User → App (clicks Sign in with Google)
2. App → Google (redirect with client_id + scopes)
3. Google → User (login + consent)
4. Google → App (authorization code via redirect)
5. App → Google (token exchange: code + client_secret → ID token + access token)
6. App parses ID token → user is signed in
