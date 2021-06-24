### hakrawler
Tags: #recon, #web_recon, #link_discovery
Link: https://github.com/hakluke/hakrawler

---
### Summary

hakrawler is a Go web crawler designed for easy, quick discovery of endpoints and assets within a web application. It can be used to discover:

-   Forms
-   Endpoints
-   Subdomains
-   Related domains
-   JavaScript files

The goal is to create the tool in a way that it can be easily chained with other tools such as subdomain enumeration tools and vulnerability scanners in order to facilitate tool chaining, for example:

```
assetfinder target.com | hakrawler | some-xss-scanner
```

### Snippets

`hakrawler -url bugcrowd.com -depth 1`

---

### References