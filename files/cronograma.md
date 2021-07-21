## CRONOGRAMA DE EXECUÇÃO

### CICLO 1

**Prazo:**
- Início: 14/06/2021
- Fim: 19/07/2021

**Descrição:** A primeira versão do sistema deve ser capaz de:
1. Capturar uma imagem no módulo a cada 60 segundos;
2. Enviar imagem do módulo para servidor através do sistema de fila de mensagens MQTT;
3. Consultar a API Vision para reconhecimento de imagem;
4. Persistir no banco de dados o resultado da consulta a API Vision;
5. Exibir em uma página HTML as informações do banco de dados;

**Etapas semanais:**

| Etapa | 1 | 2 | 3 | 4 | 5 |
|:-----:|:-:|:-:|:-:|:-:|:-:|
|   Refinamento  | X | |   |   |   | 
|   Detalhamento  | X |  |   |   |   |
|   Interface e Clientes MQTT  |  | X |   |   |   |
|   Server - Interface API Vision  |  | X |   |   |  |
|   Server - Cliente API Vision  |  | X |   |   |  |
|   Module - Interface dos Sensores  |  | X |  |   |   |
|   Module - Interface da Câmera  |  |  |  X |  X |   |
|   Module - Classe da Câmera  |  |  |  X |  X |   |
|   Server - Serviço de Identificação  |  | |  X |  X |  |
|   Server - Interface e Cliente Banco de dados  |  | |  X |  X |  |
|   Module - Controller |  |  |  X |  X |   |
|   Server - Aplicação Web |  | |  |  X |  |
|   Testes  |   |   |  | X | X |

---

### CICLO 2

**Prazo:**
- Início: 24/07/2021
- Fim: 23/08/2021

**Descrição:** A segunda versão do sistema deve ser capaz de:
1. Capturar uma imagem no módulo quando detectar movimento;
2. Coletar informações de umidade e temperatura do ambiente no momento da detecção;
3. Enviar imagem e informações do ambiente do módulo para servidor através do sistema de fila de mensagens MQTT;
4. Consultar a API Vision para reconhecimento de imagem;
5. Persistir no banco de dados o resultado da consulta a API Vision;
6. Permitir a visualização das informações do banco de dados em uma aplicação Web;
7. Oferecer filtros de pesquisa na aplicação Web para personalizar a visualização das informações do banco de dados;
8. Notificar a detecção de determinada(s) label(s) previamente configurada(s);

**Etapas semanais:**

| Etapa | 1 | 2 | 3 | 4 |
|:-----:|:-:|:-:|:-:|:-:|
|   Module - Adicionar sensores de umidade e temperatura  | X | |   |   |
|   Server - Implementar views na aplicação Web |  X |  |   |   |
|   Server - Implementar filtros na aplicação Web |   | X | X  |   |
|   Module - Adicionar sensor de presença |  | X | X |   |
|   Server - Implementar sistema de notificação  |  |  | X | X |
|   Testes  |   |   |  | X |
