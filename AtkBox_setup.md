### Attack Box Setup
Tags: #workflow, #setup
Link:

---

### Install Pre-Reqs

```
apt-get -y install parallel
```

### Axiom VPS Deployment

https://github.com/pry0cc/axiom

### Custom VPS Deployment

Start VPS

```

```

Install IVRE - https://ivre.rocks/#
```
mkdir -m 1777 var\_{lib,log}\_mongodb ivre-share
wget -q https://ivre.rocks/Vagrantfile
vagrant up --no-parallel
docker attach ivreclient
```

### BurpPro

Burp Regex for Scope Control

````
.*\.domain\.com$
````

---

### References

- https://m0chan.github.io/2019/12/17/Bug-Bounty-Cheetsheet.html
- https://github.com/pry0cc/axiom

