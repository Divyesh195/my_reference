# Cyber Security

## 1. Basic Web Vulnerabilities

### XSS - Cross-Site Scripting

Attacker injects script into your page → script runs in victim’s browser under your origin → attacker can read/modify your site’s DOM, cookies (if not HttpOnly), and make authenticated requests.

### CSRF - Cross-Site Request Forgery

Attacker causes victim’s browser to send a request to your site (e.g., via an image tag, form, or fetch from another origin) → browser automatically includes cookies → your server processes the request as if the user intended it.