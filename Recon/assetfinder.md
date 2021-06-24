### assetfinder
Tags: #recon, #web_recon, #subdomain_scraping
Link: https://github.com/tomnomnom/assetfinder

---
### Summary

Find domains and subdomains potentially related to a given domain.

#### Sources
-   crt.sh
-   certspotter
-   hackertarget
-   threatcrowd
-   wayback machine
-   dns.bufferover.run
-   facebook
    -   Needs `FB_APP_ID` and `FB_APP_SECRET` environment variables set ([https://developers.facebook.com/](https://developers.facebook.com/))
    -   You need to be careful with your app's rate limits
-   virustotal
    -   Needs `VT_API_KEY` environment variable set ([https://developers.virustotal.com/reference](https://developers.virustotal.com/reference))
-   findsubdomains
    -   Needs `SPYSE_API_TOKEN` environment variable set (the free version always gives the first response page, and you also get "25 unlimited requests") — ([https://spyse.com/apidocs](https://spyse.com/apidocs))

### Snippets

`assetfinder [--subs-only] <domain>`

---

### References