### nmap
Tags: #recon, #service_recon, #port_recon
Related to: 
See also: 
Previous:

### Body
Summary: File upload vulnerabilities occur when a file upload may be poorly implemented, as they directly access the file system, primarily this involves path traversal, however this could also cause RCEs in the case of Image Tradgik

Notes
The main vulnerabilities that file uploads face are path traversal related...

### Snippets

Expand Subnets into IPs

`nmap -sL -n -iL blocks.txt | grep 'Nmap scan report for' | cut -f 5 -d ' '`

### References
- \[\[File Upload Attacks Part 1\]\]