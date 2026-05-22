# Diagrama de Casos de Uso

# Objetivo

O Diagrama de Casos de Uso representa as interações específicas de cada perfil operacional com o sistema SafeVision AI dentro do contexto industrial do Metaindústria.

A modelagem foi segmentada por responsabilidade operacional, permitindo identificar claramente:

- ações do Operador Industrial
- responsabilidades do Supervisor de Segurança
- funcionalidades estratégicas do Gestor Industrial
- automações executadas pelo sistema

---

# Diagrama de Casos de Uso — Operador Industrial

```mermaid
flowchart LR

Operador[Operador Industrial]

subgraph SafeVisionAI [Sistema SafeVision AI]

UC1((Ser Monitorado))
UC2((Utilizar EPIs Obrigatorios))
UC3((Executar Atividade Operacional))
UC4((Detectar Uso de EPIs))
UC5((Detectar Desvio Postural))
UC6((Classificar Nivel de Risco))

end

Operador --> UC1
Operador --> UC2
Operador --> UC3

UC1 -.-> UC4
UC2 -.-> UC4
UC3 -.-> UC5

UC4 -.-> UC6
UC5 -.-> UC6
```

---

# Diagrama de Casos de Uso — Supervisor de Segurança

```mermaid
flowchart LR

Supervisor[Supervisor de Seguranca]

subgraph SafeVisionAI [Sistema SafeVision AI]

UC1((Receber Alertas))
UC2((Monitorar Dashboard))
UC3((Consultar Ocorrencias))
UC4((Analisar Eventos Criticos))
UC5((Validar Conformidade))
UC6((Emitir Alertas em Tempo Real))
UC7((Atualizar Dashboard))
UC8((Registrar Eventos))
UC9((Armazenar Historico))

end

Supervisor --> UC1
Supervisor --> UC2
Supervisor --> UC3
Supervisor --> UC4
Supervisor --> UC5

UC6 -.-> UC1
UC7 -.-> UC2
UC8 -.-> UC3
UC8 -.-> UC4
UC9 -.-> UC5
```

---

# Diagrama de Casos de Uso — Gestor Industrial

```mermaid
flowchart LR

Gestor[Gestor Industrial]

subgraph SafeVisionAI [Sistema SafeVision AI]

UC1((Visualizar Indicadores))
UC2((Gerar Relatorios))
UC3((Exportar Relatorios))
UC4((Analisar Desempenho SST))
UC5((Acompanhar Historico))
UC6((Consolidar Indicadores))
UC7((Armazenar Historico))
UC8((Registrar Eventos))

end

Gestor --> UC1
Gestor --> UC2
Gestor --> UC3
Gestor --> UC4
Gestor --> UC5

UC6 -.-> UC1
UC8 -.-> UC2
UC2 -.-> UC3
UC1 -.-> UC4
UC7 -.-> UC5
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