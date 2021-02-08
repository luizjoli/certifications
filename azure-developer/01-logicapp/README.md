# O que seria Logic App?

Logic Apps são serviço de novem que te auxilia a angedar, automatizar, orquestrar tarefas, processos de negócio e fluxos de trabalho.
Simplifica a lógica de integração de diversos serviços através de connectors, actions e events.

Todo o fluxo se inicia através de um gatilho, que é acionado quando um evento ocorre. Esses gatilhos são fornecidos pelos conectores, que podem ser agendamento simples, ou tarefas complexas de outro serviços de terceiros (Slack, Twitter, entre outros). Cada vez que a trigger é acionada uma instância do aplicativo lógico e executa o workflow.

A configuração desse fluxo pode ser feita por uma parte gráfica ou por configuração em JSON, dispensando utilização de códigos de programação.

Termos chaves:
 * Workflow: fluxo de trabalho que será executado no Logic App
 * Managed Connectors: Conectores gerenciados pela MS que foram projetados para conectar, acessar e manipular seus dados
 * Triggers: Evento que inicia a criação de uma instância do Logic app e inicia o workflow
 * Actions: Etapas que ocorrem depois que um trigger é disparado.
 * EIP (Enterprise Integration Pack): util para integrações mais avançadas.

[01 - Criando um Logic App](01-CiarLogicApp.md)

[02 - Criando um Conector Personalizado ](02-CriarConnectorPersonalizado.md)