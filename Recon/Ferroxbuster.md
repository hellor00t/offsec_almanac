### feroxbuster
Tags: #recon, #web_recon, #link_discovery
Link: https://github.com/epi052/feroxbuster

---
### Summary: 

`feroxbuster` is a tool designed to perform [Forced Browsing](https://owasp.org/www-community/attacks/Forced_browsing).

Forced browsing is an attack where the aim is to enumerate and access resources that are not referenced by the web application, but are still accessible by an attacker.

### Snippets

To run the tool on a target, just use the following command:

```
feroxbuster -u http://127.1 --insecure --proxy http://127.0.0.1:8080 -w wordlist
```

---

### References