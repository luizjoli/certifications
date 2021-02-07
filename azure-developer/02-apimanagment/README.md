# API Managment

API Managment auxlia na organização a gerenciar e produtizar API's para uma organização. É um conjunto de componentes que auxilia na criação de ciclo de vidas de API, produtos, controle de acesso, políticas de uso, segurança, cache entre outros.

Dentro os componentes que compõe o API Managment estão:

* API Gateway: 
  * Centralizador de chamadas da API
  * Verificação de credenciais
  * Utilização de Qotas e limites
  * Transformação da sua API (Ex.: XML para JSON) sem alteração de código
  * Cache para fazer sua API performar
  * Configuração de Logs
* Azure Portal:
  * Gerenciamento de criação e importação de API's
  * Criação de produto baseado nas API's
  * Configuração de políticas
  * Análise de métricas
  * Gerencia de usuários
* Portal do Desenvolvedor
  * Documentação das API's
  * Experimentação da API
  * Criação de conta e inscrição para obter chave de acesso
  * Acesso as metricas de consumo de utilização

Alem dos componentes citados acima existem também, **Produtos**, que são o empacotamento de API's para a disponibilização para os desenvolvedores. Podendo ser aberto ou protegido. Já **Grupos** que tem a responsabilidade gerenciar os produtos para os desenvolvedores, por padrão existem três grupos (administrador, desenvolvedores e convidados). Você pode personalizar novos grupos e associar com Azure Actuve Directory. Também existem os **Desenvolvedores** que serão os usuários da API's portanto, vão pertencer a grupos e possuir produtos para consumir. Por fim temos **Políticas** que são configurações que podem ser feitas a nível de API's as mais comuns, são conversão de XML para JSON, limitação de chamadas entre outras.