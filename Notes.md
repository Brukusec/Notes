# **Tools**

## Subdomains Enumeration



- Assetfinder 
  - https://github.com/tomnomnom/assetfinder
- Amass
  - https://github.com/OWASP/Amass
- Subfinder
  - https://github.com/projectdiscovery/subfinder
- Aquatone
  - https://github.com/michenriksen/aquatone
- Chaos.projectdiscovery.io
  - https://chaos.projectdiscovery.io/#/
- Securitytrails.com
  - https://securitytrails.com/
- OneforAll
  - https://github.com/shmilylty/OneForAll/



#### Examples scripts & commands

```bash
subfinder -d dominio | httpx -silent | githound
```

```bash
subfinder -d $1 -silent | httpx -silent | xargs -I %% bash -c 'python3 /root/../SecretFinder.py -i %% -e -o cli'
```

```bash
subfinder -d domainio -silent | httpx -silent | nuclei -t ../nuclei-templates/cves/ -o fileout
```

```bash
subfinder -d $ -silent | httpx -silent | nuclei -t ../nuclei-templates/ -o $2
```

```bash
cat $1 | httpx -follow-redirects -status-code -vhost -threads 100 | sort -u | grep "[200}" | cut -d [ -f1 | uniq | tee $2
```

## Intel Gathering

- Amass
  - https://github.com/OWASP/Amass
- Whois
  - https://whois.net/
- Shodan
  - https://www.shodan.io/
- Github
  - https://github.com/
- Search Engine

### Examples Shodan

Shodan search : org:organização
				hostname: dominio
				
				

## Directory Bruteforcing/Content Discovery

- dirsearch
  - https://github.com/maurosoria/dirsearch
- fuff
  - https://github.com/ffuf/ffuf
- gospider
  - https://github.com/jaeles-project/gospider
- gobuster
  - https://github.com/OJ/gobuster



## Subdomain TakeOvers

- Subjack
  - https://github.com/haccer/subjack
- Aquatone
  - https://github.com/michenriksen/aquatone
- Tko-subs
  - https://github.com/anshumanbh/tko-subs
- Can-i-takeover-xyz (manual)
  - https://github.com/EdOverflow/can-i-take-over-xyz



## Parameter Discovery

- Arjun
  - https://github.com/s0md3v/Arjun
- ParamSpider
  - https://github.com/devanshbatham/ParamSpider



## PortScan

- NMap
  - https://nmap.org/
- Masscan
  - https://github.com/robertdavidgraham/masscan
- Naabu
  - https://github.com/projectdiscovery/naabu



## Github Recon/Leak Finding

- Githound
  - https://github.com/tillson/git-hound
- Secret Finder
  - https://github.com/m4ll0k/BurpSuite-Secret_Finder
- gitrob
  - https://github.com/michenriksen/gitrob
- Trufflehog
  - https://github.com/dxa4481/truffleHog



## JS Link Analysers

- JS-Scan
  - https://github.com/zseano/JS-Scan
- Burp JS Link finder
  - https://github.com/PortSwigger/js-link-finder
- Link Finder
  - https://github.com/GerbenJavado/LinkFinder



## Useful Scripts & Tools to Automate Recon

- Httprobe
  - https://github.com/tomnomnom/httprobe
- Waybackurls
  - https://github.com/tomnomnom/waybackurls
- Tomnomnom Hacks
  - https://github.com/tomnomnom/hacks
- gwen001/pentest-tools
  - https://github.com/gwen001/pentest-tools
- Hakluke's Scripts (Hakrawler and others)
  - https://github.com/lc/hacks
  - https://github.com/hakluke
  - https://github.com/hakluke/hakrawler
- dalfox
  - https://github.com/hahwul/dalfox
- GF
  - https://github.com/tomnomnom/gf
- GAU
  - https://github.com/lc/gau
- S3Scanner
  - https://github.com/sa7mon/S3Scanner
- AWSBucketDump
  - https://github.com/jordanpotti/AWSBucketDump



## Online Services & Search Engines

- Shodan
  - https://www.shodan.io/
- Censys
  - https://censys.io/
- Fofa.so
  - https://fofa.so/
- BinaryEdge
  - https://www.binaryedge.io/
- Google/Bing/DuckDuckGo
  - https://www.google.com/
  - https://www.bing.com/
  - https://duckduckgo.com/
- Github/bitBucket Search
  - https://github.com/gwen001/github-search
- Hardenize.io
  - https://www.hardenize.com/
- Httpstatus.io
  - https://httpstatus.io/
- Mxtoolbox.com
  - https://mxtoolbox.com/
- Postb.in
  - https://postb.in/
- Crunchbase
  - https://www.crunchbase.com/
- Owler
  - https://www.owler.com/company/search-inc



## Auto Recon

- Sudomy
  - https://github.com/Screetsec/Sudomy
- TotalRecon
  - https://github.com/vitalysim/totalrecon
- OSMEDEUS 
  - https://github.com/j3ssie/Osmedeus
- Nuclei
  - https://github.com/projectdiscovery/nuclei
- Nettacker
  - https://github.com/zdresearch/OWASP-Nettacker/wiki#introduction