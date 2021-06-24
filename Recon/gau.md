### gau
Tags: #recon, #web_recon, #subdomain_scraping
Link: https://github.com/lc/gau

---
### Summary

getallurls (gau) fetches known URLs from AlienVault's Open Threat Exchange, the Wayback Machine, and Common Crawl for any given domain. Inspired by Tomnomnom's waybackurls.

### Snippets
```
printf example.com | gau
cat domains.txt | gau -t 5
gau example.com
gau -o example-urls.txt example.com
gau -b png,jpg,gif example.com
```
---

### References