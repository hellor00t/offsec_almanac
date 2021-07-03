### nuclei
Tags: #recon, #web_recon, #webapp_recon, #vuln_scan
Link: https://github.com/projectdiscovery/nuclei

---
### Summary

Nuclei is used to send requests across targets based on a template leading to zero false positives and providing fast scanning on large number of hosts. Nuclei offers scanning for a variety of protocols including TCP, DNS, HTTP, File, etc. With powerful and flexible templating, all kinds of security checks can be modelled with Nuclei.

nuclei templates are installed in $HOME/nuclei-templates/

### Snippets
Scanning for CVEs on given list of URLs.
```
nuclei -update-templates
nuclei -l target_urls.txt -t cves/

```

---

### References
https://github.com/geeknik/the-nuclei-templates
https://rayvyn.net/nuclei