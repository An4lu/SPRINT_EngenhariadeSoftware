# Diagrama de Casos de Uso

# Objetivo

O Diagrama de Casos de Uso representa as interações específicas de cada perfil operacional com o sistema SafeVision AI dentro do contexto industrial do Metaindústria.

A modelagem foi segmentada por responsabilidade operacional, permitindo identificar claramente:

- ações do Operador Industrial
- responsabilidades do Supervisor de Segurança
- funcionalidades estratégicas do Gestor Industrial
- automações executadas pelo sistema

---

# Diagrama UML — Casos de Uso

```mermaid
flowchart LR

%% ATORES

Operador[Operador Industrial]
Supervisor[Supervisor de Seguranca]
Gestor[Gestor Industrial]

%% SISTEMA

subgraph SafeVisionAI [Sistema SafeVision AI]

%% OPERADOR

UC1((Ser Monitorado))
UC2((Utilizar EPIs Obrigatorios))
UC3((Executar Atividade Operacional))

%% SUPERVISOR

UC4((Receber Alertas))
UC5((Monitorar Dashboard))
UC6((Consultar Ocorrencias))
UC7((Analisar Eventos Criticos))
UC8((Validar Conformidade Operacional))

%% GESTOR

UC9((Visualizar Indicadores))
UC10((Gerar Relatorios))
UC11((Exportar Relatorios))
UC12((Analisar Desempenho de SST))
UC13((Acompanhar Historico Industrial))

%% SISTEMA

UC14((Detectar Uso de EPIs))
UC15((Detectar Desvio Postural))
UC16((Classificar Nivel de Risco))
UC17((Registrar Eventos))
UC18((Atualizar Dashboard))
UC19((Armazenar Historico))
UC20((Emitir Alertas em Tempo Real))

end

%% RELACIONAMENTOS OPERADOR

Operador --> UC1
Operador --> UC2
Operador --> UC3

%% RELACIONAMENTOS SUPERVISOR

Supervisor --> UC4
Supervisor --> UC5
Supervisor --> UC6
Supervisor --> UC7
Supervisor --> UC8

%% RELACIONAMENTOS GESTOR

Gestor --> UC9
Gestor --> UC10
Gestor --> UC11
Gestor --> UC12
Gestor --> UC13

%% FLUXOS INTERNOS

UC1 -.-> UC14
UC2 -.-> UC14

UC3 -.-> UC15

UC14 -.-> UC16
UC15 -.-> UC16

UC16 -.-> UC17
UC17 -.-> UC18
UC17 -.-> UC19
UC16 -.-> UC20

UC20 -.-> UC4
UC18 -.-> UC5

UC19 -.-> UC6
UC19 -.-> UC13

UC17 -.-> UC10
UC10 -.-> UC11

UC18 -.-> UC9
UC9 -.-> UC12
```

---

# Casos de Uso por Ator

---

# Operador Industrial

| Caso de Uso | Objetivo |
|---|---|
| Ser Monitorado | Permitir acompanhamento contínuo das atividades operacionais |
| Utilizar EPIs Obrigatórios | Garantir conformidade de segurança |
| Executar Atividade Operacional | Realizar tarefas industriais monitoradas |

---

# Supervisor de Segurança

| Caso de Uso | Objetivo |
|---|---|
| Receber Alertas | Ser notificado sobre riscos operacionais |
| Monitorar Dashboard | Acompanhar eventos em tempo real |
| Consultar Ocorrências | Verificar eventos registrados |
| Analisar Eventos Críticos | Avaliar situações de risco |
| Validar Conformidade Operacional | Garantir cumprimento das normas de SST |

---

# Gestor Industrial

| Caso de Uso | Objetivo |
|---|---|
| Visualizar Indicadores | Acompanhar métricas estratégicas |
| Gerar Relatórios | Consolidar dados operacionais |
| Exportar Relatórios | Compartilhar informações gerenciais |
| Analisar Desempenho de SST | Avaliar indicadores de segurança |
| Acompanhar Histórico Industrial | Verificar evolução operacional |

---

# Processos Automatizados do Sistema

| Processo | Objetivo |
|---|---|
| Detectar Uso de EPIs | Identificar conformidade automaticamente |
| Detectar Desvio Postural | Identificar riscos ergonômicos |
| Classificar Nível de Risco | Determinar criticidade operacional |
| Registrar Eventos | Armazenar ocorrências |
| Atualizar Dashboard | Atualizar informações em tempo real |
| Armazenar Histórico | Garantir rastreabilidade |
| Emitir Alertas em Tempo Real | Reduzir tempo de resposta operacional |

---

# Benefícios da Modelagem

- separação clara de responsabilidades
- melhor rastreabilidade operacional
- alinhamento com contexto industrial real
- coerência entre requisitos e arquitetura
- aderência ao modelo de segurança proativa
- suporte à tomada de decisão estratégica