### unfurl
Tags: #recon, #wordlists
Link: https://github.com/tomnomnom/unfurl

---
### Summary

getallurls (gau) fetches known URLs from AlienVault's [Open Threat Exchange](https://otx.alienvault.com), the Wayback Machine, and Common Crawl for any given domain. Inspired by Tomnomnom's [waybackurls](https://github.com/tomnomnom/waybackurls).

### Snippets
You can extract the domains from the URLs with the `domains` mode, if you don't want to output duplicate values you can use the `-u` or `--unique` flag:

```
cat urls.txt | unfurl --unique domains
```
Paths

```
▶ cat urls.txt | unfurl paths
/users
/orgs
/about
```

Query String Keys

```
▶ cat urls.txt | unfurl keys
id
name
org
```

Query String Values

```
▶ cat urls.txt | unfurl values
123
Sam
ExCo
```

Query String Key/Value Pairs

```
▶ cat urls.txt | unfurl keypairs
id=123
name=Sam
org=ExCo
```

---

### References

* https://tomnomnom.com/talks/wwwww.pdf