# ASNFinder
ASNFinder is a tool created in Python3 that searches for ASNS in domains and organizations.

# Versão
```sh
0.2
```

# Update
Argumentos -asn e -ips<br>
Argumento -d e -asn

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
<li>This command gets the domain and finds information like asns, org, cidr, etc...</li>
```sh
./asnfinder -d yahoo.com

ASN: 36647
ASN_CIDR: 98.137.11.0/24
ASN_ORG: YAHOO-GQ1, US
```

# Argument -asm
<li>This command checks the ASN and org cidrs</li>
```sh
./asnfinder -asn AS7233

"7233","YAHOO-, US"
2001:4998:ef60::/48
2001:4998:ef61::/48
209.131.48.0/23
98.136.0.0/23
```

# Catching ASNs and IPs
```sh
./asnfinder -o yahoo -asns
./asnfinder -o yahoo -ips
```
