### Wordlist Workflow
Tags: #workflow
Link:

### Gather URLs

1) Your Burp Suite history is a good source

	`Target tab > Site map -> Right click a host -> 'Copy URLs in this host'`

2) Copy to file `urls.txt`

	Run TLD's through [Wordlists/gau](Wordlists/gau.md)

	`gau example.net | unfurl -u paths > paths.txt`

	OR

	`cat urls.txt | unfurl -u paths > paths.txt`

Extract parts of the path

	`sed 's#/#\n#g' paths.txt | sort -u > endpoints`

Extract keys

	`gau example.net | unfurl -u keys`
	
	
Remove up to last backslash from URL
	
`sed 's/^.*[/]//' paths.txt > endpoints.txt`

### One-Liners

```
echo "bugcrowd.com" | subfinder -silent | hakrawler -plain -usewayback -scope yolo | sed $'s/[./?=:&#]/\\\n/g' | anew
```

A quick one-liner that will gather + crawl all subdomains, then convert to a custom wordlist unique to that organisation based on discovered URLs!

```
subfinder -d bugcrowd\[.\]com -silent | httpx -silent | hakrawler -plain | tr "\[:punct:\]" "\\n" | sort -u
```

---
### References
* https://tomnomnom.com/talks/wwwww.pdf
* https://twitter.com/hakluke/status/1301487471704776705
* https://twitter.com/bugcrowd/status/1362627992036519940
* https://github.com/payloadbox
* https://github.com/swisskyrepo/PayloadsAllTheThings
* https://github.com/danielmiessler/SecLists