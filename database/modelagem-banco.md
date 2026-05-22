# Modelagem do Banco de Dados

# Objetivo

A modelagem do banco de dados foi estruturada para garantir rastreabilidade operacional, histórico de conformidade e gerenciamento de eventos críticos industriais.

---

# Entidades Principais

## operadores

Armazena dados dos operadores monitorados pelo sistema.

## setores

Representa as áreas da planta industrial.

## cameras

Gerencia dispositivos responsáveis pela captura do fluxo de vídeo.

## tipos_epi

Lista os equipamentos de proteção monitorados.

## deteccoes_epi

Armazena inferências realizadas pela Visão Computacional.

## eventos_risco

Registra ocorrências críticas detectadas pelo sistema.

## conformidade_diaria

Consolida métricas e indicadores operacionais.

## relatorios

Armazena exportações analíticas e históricos gerenciais.

---

# Objetivos da Modelagem

- Garantir rastreabilidade
- Armazenar histórico operacional
- Consolidar indicadores industriais
- Permitir auditoria de conformidade
- Suportar relatórios analíticos
- Apoiar tomada de decisão