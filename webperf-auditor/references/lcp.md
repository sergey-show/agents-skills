# LCP fix map

| Bottleneck | First fixes |
|------------|-------------|
| Resource load delay | real `src`, `fetchpriority=high`, preload, no lazy on LCP |
| Render delay | critical CSS, defer JS, SSR/HTML present, break long tasks |
| Load duration | AVIF/WebP, srcset, CDN, cache headers, font-display swap |
| TTFB | fewer redirects, faster origin, edge cache, bfcache eligibility |
