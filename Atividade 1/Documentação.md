# Criação de Container - Zabbix Proxy SQLite 5.2.0 <h1>

- Comando para criação do container via console Docker:

docker run --name some-zabbix-proxy-sqlite3 \
	-e ZBX_HOSTNAME=some-hostname \
	-e ZBX_SERVER_HOST=some-zabbix-server \
	-e ZBX_STARTPOLLERS=50 \
	-e ZBX_STARTPREPROCESSORS=10 \
	-e ZBX_STARTPOLLERSUNREACHABLE=50 \
	-e ZBX_STARTTRAPPERS=50 \
	-e ZBX_STARTPINGERS=50 \
	-e ZBX_STARTDISCOVERERS=5 \
	-e ZBX_CACHESIZE=16M \
	-e ZBX_CONFIGFREQUENCY=180 \
	-e ZBX_ENABLEREMOTECOMMANDS=1 \
	-e ZBX_STARTHTTPPOLLERS=10 \
	-p 10051:10051 \
	-d ugoclemes/zabbix-proxy-5.2.0:latest

- Acesso a console do container e instalação do driver ODBC FreeTDS e editado o arquivo /etc/odbc.ini para configuração de comunicação com Banco de Dados.


