# Zabbix com Docker Compose
Este repositório sobe um ambiente Zabbix completo (MySQL, Zabbix Server e Frontend Web) utilizando Docker Compose.
## Dependências
```bash
sudo apt update -y
git clone https://github.com/eliezershell/docker.git
chmod +x ./docker/instalador_docker.sh
./docker/instalador_docker.sh
```

## Gerando Certificado TLS/SSL
```bash
openssl req -x509 -nodes -days 365 \
-newkey rsa:2048 \
-keyout privkey.pem \
-out cert.pem \
-subj "/C=BR/ST=Sao Paulo/L=Hortolandia/O=Eliezer Inc./OU=Observability/CN=zabbix.eliezer.cloud" \
-addext "subjectAltName=DNS:zabbix.eliezer.cloud"
```
## Subindo os containers
```bash
git clone https://github.com/eliezershell/zabbix.git
cd zabbix
docker compose up -d
```
