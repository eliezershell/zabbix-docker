# Zabbix com Docker Compose
Este repositório sobe um ambiente Zabbix completo para TESTES (MySQL, Zabbix Server e Frontend Web) utilizando Docker Compose.
## Dependências
```bash
git clone https://github.com/eliezershell/docker.git
bash ./docker/install.sh
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
docker compose up -d
```
