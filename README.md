# SafeVision AI

## Sistema Inteligente de Segurança Proativa Industrial

### Challenge 2026 — FIAP × SPI Integrações

---

# Integrantes

- Ana Luiza Oliveira Dourado — RM558793
- Carlos Augusto da Cruz Possi — RM558758
- Fabio Henrique Santos Faria — RM552453
- João Pedro Bernardes Santos da Silva — RM557142
- Leonardo Tanaka Cortez — RM556781

Professor Responsável:
- Hercules Lima Ramos

---

# Sobre o Projeto

O SafeVision AI é uma solução inteligente voltada ao contexto industrial do Metaindústria, desenvolvida com foco em segurança proativa, monitoramento contínuo e prevenção de acidentes em ambientes fabris.

A proposta utiliza Inteligência Artificial, Visão Computacional e análise em tempo real para automatizar o gerenciamento de segurança operacional, realizando o monitoramento do uso de Equipamentos de Proteção Individual (EPIs) e a identificação de riscos ergonômicos em atividades industriais.

O sistema atua diretamente no chão de fábrica, auxiliando supervisores e gestores através de alertas instantâneos, análise de conformidade e geração de dados estratégicos para tomada de decisão.

---

# Problema Abordado

Ambientes industriais apresentam riscos constantes relacionados ao uso inadequado de EPIs, falhas operacionais e execução incorreta de atividades físicas repetitivas.

Grande parte das empresas ainda depende de fiscalização manual realizada por supervisores ou técnicos de segurança, criando limitações críticas como:

- ausência de monitoramento contínuo
- cobertura limitada das áreas industriais
- demora na identificação de irregularidades
- falhas humanas de observação
- ausência de rastreabilidade inteligente
- dificuldade na prevenção de acidentes
- aumento de afastamentos ergonômicos
- crescimento de passivos trabalhistas

Além disso, o modelo tradicional atua de forma reativa, respondendo apenas após a ocorrência de acidentes ou incidentes.

O desafio do projeto consiste em transformar esse cenário em uma cultura de segurança preventiva baseada em dados e inteligência operacional.

---

# Proposta de Solução

O SafeVision AI atua como um sistema inteligente de monitoramento operacional industrial.

A solução utiliza câmeras instaladas no ambiente fabril para capturar fluxos contínuos de vídeo que são processados em tempo real através de modelos de Visão Computacional.

A plataforma é capaz de:

- detectar automaticamente ausência de EPIs
- identificar riscos ergonômicos
- reconhecer posturas inadequadas
- monitorar movimentação em áreas críticas
- emitir alertas instantâneos
- registrar eventos de risco
- gerar histórico de conformidade
- consolidar indicadores industriais

Quando uma irregularidade é detectada, o sistema realiza:

1. inferência computacional
2. validação de regras de negócio
3. classificação do nível de risco
4. registro da ocorrência
5. envio de alerta operacional
6. atualização do dashboard em tempo real

A proposta promove a transição da segurança reativa para um modelo preventivo e proativo.

---

# Objetivo Geral

Desenvolver uma solução inteligente de monitoramento industrial capaz de automatizar o gerenciamento de EPIs e detectar riscos operacionais em tempo real através de Inteligência Artificial e Visão Computacional.

---

# Objetivos Específicos

- Automatizar o monitoramento de EPIs
- Detectar irregularidades operacionais
- Identificar riscos ergonômicos
- Emitir alertas em tempo real
- Consolidar dados históricos de conformidade
- Reduzir acidentes industriais
- Auxiliar supervisores na tomada de decisão
- Promover cultura de prevenção
- Melhorar indicadores de segurança operacional

---

# Tecnologias Selecionadas

| Tecnologia | Finalidade |
|---|---|
| Python | Processamento de IA e integração |
| YOLO26 | Detecção de objetos em tempo real |
| OpenCV | Processamento computacional de imagem |
| FastAPI | Comunicação entre serviços |
| PostgreSQL | Persistência e rastreabilidade |
| React | Dashboard operacional |
| TypeScript | Organização e escalabilidade |
| WebSockets | Atualizações instantâneas |

---

# Justificativa Técnica

A arquitetura tecnológica foi definida considerando os requisitos do contexto industrial do Metaindústria.

## Tempo Real

A utilização de WebSockets permite atualização imediata dos dashboards operacionais.

## Escalabilidade

A separação modular dos componentes permite crescimento progressivo do sistema industrial.

## Confiabilidade

O PostgreSQL garante integridade e rastreabilidade dos eventos registrados.

## Performance

O modelo YOLO26 oferece alta velocidade de inferência computacional.

## Flexibilidade

A utilização de APIs desacopladas permite integração futura com novos módulos industriais.

## Monitoramento Contínuo

A combinação entre OpenCV e IA possibilita análise constante dos fluxos de vídeo.

---

# Funcionalidades Principais

- Monitoramento contínuo de EPIs
- Detecção postural
- Alertas operacionais
- Dashboard em tempo real
- Histórico de conformidade
- Classificação de risco
- Gestão de eventos críticos
- Relatórios analíticos
- Indicadores operacionais

---

# Estrutura Documental

## Levantamento de Requisitos

- docs/levantamento-requisitos.md

## Escopo do Projeto

- docs/escopo-do-projeto.md

## Arquitetura da Solução

- docs/arquitetura-da-solucao.md

## Personas

- docs/personas.md

## Regras de Negócio

- docs/regras-de-negocio.md

---

# Diagramas UML

## Diagrama de Casos de Uso

- docs/diagramas/casos-de-uso.md

## Diagrama de Atividades

- docs/diagramas/atividades.md

## Diagrama de Classes

- docs/diagramas/classes.md

---

# Modelagem do Banco de Dados

- database/modelagem-banco.md

---

# Status do Projeto

🚧 Sprint 1 — Engenharia e documentação da solução