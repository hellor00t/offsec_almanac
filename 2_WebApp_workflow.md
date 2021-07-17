### WebApp Workflow
Tags: #workflow

---

### Web Enumeration

#### Service Recon

[nmap](Recon/nmap)

#### Subdomain Scraping & Crawling

[amass](Recon/amass)
[assetfinder](Recon/assetfinder)

`amass enum -d ebay.com | hakrawler > urls.txt`

Note: Clean Output - Need to fix above synatx

`cat urls.txt | cut -d " " -f 2 > urls_cleaned.txt`

 Send output to [Burpsuite](Recon/Burpsuite)

`cat crawl.txt | parallel -j 100 curl --proxy http://127.0.0.1:8080 -sk > /dev/null`

#### Link Discovery

Create domain list off of Subdomain & Scraping

`cat urls_cleaned.txt | unfurl --unique domains > domains.txt`

Create a [wordlist](5_Wordlist_workflow.md) using known endpoints as a seed. Then use [Ferroxbuster](Recon/Ferroxbuster)to discover more endpoints.

#### Subdomain Validation

`cat targets.txt | aquatone`

OR

`cat hosts.txt | httpx`

---

### References

* https://pbs.twimg.com/media/EfMa-dyXgAcRqjx?format=jpg&name=large

* ![Image](https://pbs.twimg.com/media/EfMa-dyXgAcRqjx?format=jpg&name=large)

* https://raw.githubusercontent.com/imran-parray/Mind-Maps/master/Bug%20Hunters%20Methodology%20v4/MindMap.png

* ![https://raw.githubusercontent.com/imran-parray/Mind-Maps/master/Bug%20Hunters%20Methodology%20v4/MindMap.png](https://raw.githubusercontent.com/imran-parray/Mind-Maps/master/Bug%20Hunters%20Methodology%20v4/MindMap.png)

* https://project-awesome.org/qazbnm456/awesome-web-security