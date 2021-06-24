### naabu
Tags: #recon, #port_recon
Related to: 
See also: 
Previous:
Link: https://github.com/projectdiscovery/naabu

---
### Summary: 

Naabu is a port scanning tool written in Go that allows you to enumerate valid ports for hosts in a fast and reliable manner. It is a really simple tool that does fast SYN/CONNECT scans on the host/list of hosts and lists all ports that return a reply.

Notes
The main vulnerabilities that file uploads face are path traversal related...

### Snippets

To run the tool on a target, just use the following command:
`naabu -host hackerone.com`

The ports to scan for on the host can be specified via `-p` parameter. It takes nmap format ports and runs enumeration on them.

`naabu -p 80,443,21-23 -host hackerone.com`

The ports discovered can be piped to other tools too. For example, you can pipe the ports discovered by naabu to `httpx` which will then find running http servers on the host.

`echo hackerone.com | naabu -silent | httpx -silent`

Integrated nmap support with `nmap` and `nmap-cli` flag, in config file you can define any `nmap` command you wish to run on the result of naabu, make sure you have `nmap` installed to use this feature.

`echo hackerone.com | naabu -nmap-cli 'nmap -sV -oX naabu-output'`

---

### References