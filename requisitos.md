# Requisitos do Sistema
> Descrição dos requisitos do sistema.



1. [Entradas.](#1-.-entradas)
2. [Saídas.](#saídas)
3. [Funcionalidades.](#funcionalidades)
4. [Requisitos não funcionais.](#requisitos-não-funcionais)
5. [Restrições.](#restrições)

---

### 1. Entradas

* Sinal de detecção de movimento.
* Medidas de temperatura.
* Medidas de umidade.
* Fotografia do local.
* Localização dos módulos.
* Fonte de tempo.

### 2. Saídas

* Relatório com informações de monitoramento:
  * Animal detectado.
  * Temperatura.
  * Umidade.
  * Local.
  * Horário.
* Consultas das informações.
* Notificações de animais detectados.

### 3. Funcionalidades

* Permitir a detecção de movimento das espécies faunísticas do ambiente monitorado.
* Capturar fotografias do ambiente após a detecção do movimento.
* Efetuar a leitura de temperatura e umidade do ambiente para cada captura de fotografia.
* Realizar a identificação das espécies com base nas fotografias capturadas.
* Armazenar as fotografias das espécies identificadas e informações do ambiente.
* Disponibilizar relatórios através de uma aplicação web com as seguintes informações:
  * Animais identificados, localização do módulo, horário da detecção, temperatura e umidade do local
* Permitir consultas, via aplicação web, das informações armazenadas com a utilização de filtros específicos (por espécie, por período). 
* Gerar notificação após detecção e identificação da espécie.

### 4. Requisitos não funcionais

* **Desempenho:** o servidor deve identificar o animal em até 1 minuto após receber a fotografia; As capturas devem ser enviadas para o servidor num ciclo de 10 minutos ou lotes de 50 fotografias.
* **Energia:** as fontes de energia dos módulos devem ser compostas por baterias carregadas através de painel fotovoltaico.  
* **Usabilidade:** relatório com informações das espécies identificadas e do ambiente devem ser disponibilizados através da internet.

### 5. Restrições

* O servidor deve utilizar a API Vision do Google para identificação das espécies através das fotografias capturadas pelos módulos.



