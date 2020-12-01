4) A equipe de desenvolvimento XPTO deseja monitorar aplicação web de votação, composta de:

- Frontend
    * Monitoramento via WebCenarário validando codigo da pagina, tempo de resposta, tempo de download e autenticação.

- Backend
    * Monitoramento de disponibilidade de serviços, comunicação TCP/UDP e recursos de infraestrutura.

- Banco de dados
    * Monitoramento de disponibilidade dos serviços, comunicação TCP, disponibilidade e status do Banco de Dados

- Recebe os votos e os insere no banco de dados
- Lista as votações e resultados
- Controla as votações em aberto, opções de cada votação e resultado agregado (parcial ou definitivo)
    * Inserir os dados no Banco, onde será possivel a coleta através do Zabbix via ODBC, assim sendo possivel a criação de Dashboard, acionamentos por Telegram, Teams e/ou E-mail
- Interface para visualizar votações e enviar votos
    * Criação de Dasboard via Grafana de todos os recursos monitorado e disponibilizar para acesso.

- Essa aplicação está em desenvolvimento e a equipe precisa de auxílio da equipe de monitoração para desenvolver as métricas que serão coletadas. O que você sugere para cada componente e para o serviço como um todo
