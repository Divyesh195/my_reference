# All About Authentication

## 1. Cookies

### HttpOnly
Prevents JavaScript from reading the cookie through [document.cookies]. <br>
However, the browser still sends the cookie automatically with matching fetch, XHR, form, and navigation requests. Therefore, HttpOnly protects the token’s confidentiality from JavaScript, but it does not by itself prevent CSRF or stop an XSS attack from making authenticated requests.

### Secure
Secure tells the browser to send the cookie only over HTTPS.

### Samesite
SameSite controls whether the browser sends a cookie with requests initiated from another site. It provides partial protection against CSRF. A site is not exactly the same as an origin: origins also include port.

sameSite: "strict" --> The cookie is sent only for same-site requests.

SameSite=Lax --> The cookie is sent for same-site requests and certain cross-site top-level navigations, generally involving safe methods such as GET.

SameSite=None --> The cookie is sent with both same-site and cross-site requests.