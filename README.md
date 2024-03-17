# ASNFinder
ASNFinder é uma Ferramenta escrita em Python3 que busca por ASNS e IPS de uma organização

# Versão
```sh
0.2
```

# Atualização
Argumentos -asn e -ips
Argumento -d e -asn

# Instalação
```sh
git clone https://github.com/yHunterDep/asnfinder
cd asnfinder
pip3 install -r requirements.txt
chmod +x asnfinder
```
# Help do ASNfinder
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

# Usando o ASNfinder
```sh
./asnfinder -o yahoo
./asnfinder -o yahoo -A 'Mozilla/5.0'
```

# Argumento -d (domínio)
<l>Este comando pega o domínio e descobre o cidr, asn e org</l>
```sh
./asnfinder -d yahoo.com

ASN: 36647
ASN_CIDR: 98.137.11.0/24
ASN_ORG: YAHOO-GQ1, US
```

# Argumento -asn
<l>Este comando verifica os cidrs do ASN e org</l>
```sh
./asnfinder -asn AS7233

"7233","YAHOO-, US"
2001:4998:ef60::/48
2001:4998:ef61::/48
209.131.48.0/23
98.136.0.0/23
```

# pegando ASNs e IPs
```sh
./asnfinder -o yahoo -asns
./asnfinder -o yahoo -ips
```
