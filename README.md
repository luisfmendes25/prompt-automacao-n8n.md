# 🎯 Desafio: Planejando Automações com n8n

## 🧱 Passo 1: Defina a automação desejada

Quero criar uma automação no N8N para **abrir tickets de incidentes automaticamente a partir de alertas de infraestrutura e notificar a equipe**.

**Público ou responsável:**
Equipe de Monitoramento e Operações (NOC).

**Resultado esperado:**
Criar um ticket no sistema de gestão com os detalhes da falha e enviar uma notificação no chat da equipe sempre que um alerta crítico for disparado.

---

## 🧱 Passo 2: Adicione contexto e regras

**Ferramentas envolvidas:**
Zabbix (monitoramento), Jira (gestão de tickets) e Telegram (notificação de equipe).

**Fluxo desejado:**
1. Receber o payload do alerta (em formato JSON) disparado pelo Zabbix via Webhook.
2. Criar uma nova "Issue" no Jira contendo o nome do host, o erro e o horário.
3. Enviar uma mensagem para o grupo do NOC no Telegram contendo o link do ticket gerado no Jira.

**Regras importantes:**
Filtrar e ignorar alertas com severidade "Information" ou "Warning". A automação só deve seguir o fluxo e abrir tickets para alertas classificados como "High" ou "Disaster".

---

## 🧱 Passo 3: Prompt Final

**Atue como um especialista em N8N.**

**Crie uma automação para** abrir tickets de incidentes automaticamente a partir de alertas de infraestrutura e notificar a equipe.

**Público:** 
Equipe de Monitoramento e Operações (NOC).

**Ferramentas envolvidas:** 
Zabbix, Jira e Telegram.

**Fluxo:** 
Receber o alerta via Webhook do Zabbix, criar uma issue no Jira e enviar uma mensagem de notificação para o grupo do NOC no Telegram com o link do ticket criado.

**Regras:** 
Ignorar alertas com severidade menor que "High" (processar apenas High e Disaster).

**Explique quais nós do N8N devem ser utilizados e a lógica de funcionamento do workflow.**
