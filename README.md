# asnfinder
asnfinder é um script em python que busca por asns

# instalação
```sh
git clone https://github.com/yHunterDep/asnfinder
cd asnfinder
pip3 install -r requirements.txt
chmod +x asnfinder
```
# help do ASNfinder
```sh
./asnfinder -h

usage: asnfinder [-h] -o ORG [-A USER_AGENT]
                 [-asns] [-ips]                                                                     options:
  -h, --help            show this help message
                        and exit
  -o ORG, --org ORG     organização, ex: --org                            yahoo
  -A USER_AGENT, --user_agent USER_AGENT
                        coloque o user-agent
                        (não obrigatório)
  -asns, --asns         o ASNFinder vai trazer                            apenas os ASNS
  -ips, --ips           o ASNFinder irá trazer
                        apenas os IPs
```

# usando o ASNfinder
```sh
./asnfinder -o yahoo
./asnfinder -o yahoo -A 'Mozilla/5.0'
```

# pegando asns e ips
```sh
./asnfinder -o yahoo -asns
./asns -o yahoo -ips
```
