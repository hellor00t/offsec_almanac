### gau
Tags: #recon, #wordlists
Link: https://github.com/lc/gau

---
### Summary

getallurls (gau) fetches known URLs from AlienVault's [Open Threat Exchange](https://otx.alienvault.com), the Wayback Machine, and Common Crawl for any given domain. Inspired by Tomnomnom's [waybackurls](https://github.com/tomnomnom/waybackurls).

### Snippets

`gau -o example-urls.txt example.com`

Subdomains from Wayback Machine

`gau -subs example.com | cut -d / -f 3 | sort -u`

---

### References

* https://tomnomnom.com/talks/wwwww.pdf