# ASNFinder
ASNFinder is a tool created in Python3 that searches for ASNS in domains and organizations.

# Version
```sh
0.4
```

# Update
Domain (-d) Bug update

# Instalation
```sh
git clone https://github.com/yHunterDep/asnfinder
cd asnfinder
pip3 install -r requirements.txt
chmod +x asnfinder
```
# Help of ASNfinder
```sh
./asnfinder -h

usage: asnfinder [-h] [-o ORG] [-A USER_AGENT] [-d DOMAIN] [-asn ASN] [-asns] [-ips]

options:
  -h, --help            show this help message and exit
  -o ORG, --org ORG     organização, ex: --org yahoo
  -A USER_AGENT, --user_agent USER_AGENT
                        coloque o user-agent (não obrigatório)
  -d DOMAIN, --domain DOMAIN
                        coloque um dominio
  -asn ASN, --asn ASN   coloque um asn, ex: AS7233
  -asns, --asns         o ASNFinder vai trazer apenas os ASNS
  -ips, --ips           o ASNFinder irá trazer apenas os IPs
```

# Basic of ASNfinder (-org)
```sh
./asnfinder -o yahoo
./asnfinder -o yahoo -A 'Mozilla/5.0'
```

# Argument -d (domain)
This command gets the domain and finds information like asns, org, cidr, etc...
```sh
./asnfinder -d yahoo.com

ASN: 36647
ASN_CIDR: 98.137.11.0/24
ASN_ORG: YAHOO-GQ1, US
```

# Argument -asn
This command checks the ASN and org cidrs
```sh
./asnfinder -asn AS40342

199.47.138.0/23
104.200.221.0/24
104.200.218.0/24
8.40.122.0/24
199.47.137.0/24
```

# Catching ASNs and IPs
```sh
./asnfinder -o yahoo -asns
./asnfinder -o yahoo -ips
```
