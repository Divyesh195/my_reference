# All About Web Optimization

## 1. Image optimization

Reduce the image size and use formats like WebP, AVIF. Add responsive variants (srcset) so mobile devices download smaller images.

## 2. CDN

A CDN caches static assets (images, CSS, JS, videos) on edge servers worldwide and serves them from the server closest to the user.

## 3. Lazy loading

Lazy loading defers downloading off-screen images (and sometimes other resources) until the user scrolls near them.

## 4. Caching

Caching stores resources in the browser (and often at the CDN/edge) so repeat visits don’t re-download the same files.

## 5. Minimal HTTP requests

Each request adds overhead (DNS, TCP/TLS handshakes, headers), so fewer requests usually mean faster pages. Combine/minify CSS and JS where practical; remove unused code.
