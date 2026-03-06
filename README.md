# Zabbix com Docker Compose
Este repositório sobe um ambiente Zabbix completo (MySQL, Zabbix Server e Frontend Web) utilizando Docker Compose.
## Dependências
```bash
sudo apt update -y
git clone https://github.com/eliezershell/docker.git
chmod +x ./docker/instalador_docker.sh
./docker/instalador_docker.sh
```
## Subindo os containers
```bash
git clone https://github.com/eliezershell/zabbix.git
cd zabbix
docker compose up -d
```
