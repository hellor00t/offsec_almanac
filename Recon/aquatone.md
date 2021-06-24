### aquatone
Tags: #recon, #web_recon
Related to: 
See also: 
Previous:
Link: https://github.com/michenriksen/aquatone

---
### Summary: 

Aquatone is a tool for visual inspection of websites across a large amount of hosts and is convenient for quickly gaining an overview of HTTP-based attack surface.

Aquatone is designed to be as easy to use as possible and to integrate with your existing toolset with no or minimal glue. Aquatone is started by piping output of a command into the tool. It doesn't really care how the piped data looks as URLs, domains, and IP addresses will be extracted with regular expression pattern matching. This means that you can pretty much give it output of any tool you use for host discovery.

### Snippets

To run the tool on a target, just use the following command:

`cat targets.txt | aquatone`

Be default, Aquatone will scan target hosts with a small list of commonly used HTTP ports: 80, 443, 8000, 8080 and 8443. You can change this to your own list of ports with the `-ports` flag:

`cat hosts.txt | aquatone -ports 80,443,3000,3001`

Aquatone can make a report on hosts scanned with the [Nmap](https://nmap.org/) or [Masscan](https://github.com/robertdavidgraham/masscan) portscanner. Simply feed Aquatone the XML output and give it the `-nmap` flag to tell it to parse the input as Nmap/Masscan XML:

```
$ cat scan.xml | aquatone -nmap
```

---

### References