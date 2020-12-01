# Monitoramento de Banco de Dados SQLServer <h1>

- Criação container SQLServer e inserção de dados manualmente:
    docker run -e 'ACCEPT_EULA=Y' -e 'SA_PASSWORD=projeto_cary2020' -p 1433:1433 ugoclemes/mssql_dbjob:latest

- Acesso ao container para validação dos Dados no Banco:
    docker exec -it 9a43b69b48ae /opt/mssql-tools/bin/sqlcmd -S localhost -U sa -P projeto_cary2020

https://hub.docker.com/r/ugoclemes/mssql_dbjob

- Criado Template para monitoramento do Banco de Dados SQLServer via ODBC para coleta de Status de um JOB.
- Item para coleta do dado via ODBC.GET
- LLD para criação de Itens por JOBs com a função de Preprocessamento do item dependente.
- Criação de Triggers separando por severidade.
    https://github.com/Ugoclemes/projeto_cary/blob/main/Atividade%202/Template%20-%20SQLSever%20-%20ODBC.json

- Disponibilizado imagem Dashboard criado no Grafana
    https://github.com/Ugoclemes/projeto_cary/blob/main/Atividade%202/Grafana%20-%20Dashboard%20JOBs.JPG