# SafeVision AI

## Sistema Inteligente de Segurança Proativa Industrial

### Challenge 2026 — FIAP × SPI Integrações

---

# Integrantes

* Ana Luiza Oliveira Dourado — RM558793
* Carlos Augusto da Cruz Possi — RM558758
* Fabio Henrique Santos Faria — RM552453
* João Pedro Bernardes Santos da Silva — RM557142
* Leonardo Tanaka Cortez — RM556781

Professor Responsável:

* Hercules Lima Ramos

---

# Visão Geral do Projeto

O SafeVision AI é uma plataforma inteligente de monitoramento operacional industrial desenvolvida para atuar diretamente no contexto do Metaindústria, utilizando Inteligência Artificial, Visão Computacional e processamento em tempo real para prevenção proativa de acidentes industriais.

A solução foi concebida para transformar o modelo tradicional de segurança ocupacional, substituindo processos reativos e dependentes exclusivamente de supervisão humana por um ecossistema inteligente capaz de monitorar continuamente ambientes industriais críticos.

O sistema realiza análise automatizada de fluxos de vídeo industriais para identificação de:

* ausência de Equipamentos de Proteção Individual (EPIs)
* riscos ergonômicos
* comportamentos inseguros
* movimentações críticas
* padrões recorrentes de não conformidade
* situações de risco operacional

Além da identificação automática das irregularidades, a plataforma fornece alertas instantâneos, rastreabilidade histórica, dashboards operacionais e relatórios analíticos estratégicos voltados à gestão industrial.

---

# Sprint 2 — Prototipação Funcional e Navegável

Durante a Sprint 2 foi desenvolvido um protótipo navegável de alta fidelidade do SafeVision AI com o objetivo de validar os fluxos operacionais modelados na Sprint 1 e simular a experiência real dos usuários da plataforma.

O projeto evoluiu da documentação e modelagem para uma representação visual funcional da solução, permitindo a validação dos fluxos de negócio e da experiência do usuário.

---

## MVP Desenvolvido

Foi desenvolvido um MVP funcional em código para demonstrar a viabilidade técnica da solução e validar os principais fluxos da plataforma.

🔗 MVP:

https://sprint-2-engenharia-de-software-mvp.vercel.app/

---

## Protótipo Navegável (Figma)

Protótipo de alta fidelidade contendo as principais telas da aplicação e os fluxos operacionais definidos na Sprint 1.

🔗 Figma:

https://www.figma.com/design/T2jxOiZXGaYVfIhwDWxHow/Untitled?node-id=0-1&t=jGSRvchUXf67OWD6-1

---

## Vídeo de Apresentação

Demonstração dos fluxos principais do sistema e da aplicação da solução no contexto do desafio Metaindústria.

🎥 Vídeo:

https://youtu.be/FAV2OXlJuUw

---

# Contextualização do Problema

No cenário industrial moderno, a Segurança e Saúde do Trabalho deixou de ser apenas uma obrigação regulatória e passou a representar um fator estratégico diretamente relacionado à produtividade, continuidade operacional e sustentabilidade corporativa.

Apesar disso, grande parte das indústrias ainda utiliza processos tradicionais de fiscalização baseados em:

* inspeções manuais
* auditorias periódicas
* supervisão presencial limitada
* preenchimento manual de relatórios
* monitoramento não contínuo

Esse modelo apresenta limitações severas em ambientes industriais complexos.

## Limitações Operacionais

* impossibilidade de monitoramento integral da planta industrial
* falhas humanas de observação
* dificuldade de rastreamento histórico
* demora na identificação de riscos
* ausência de previsibilidade operacional

## Impactos Industriais

* aumento de acidentes ocupacionais
* crescimento de afastamentos ergonômicos
* redução da produtividade
* aumento de passivos trabalhistas
* elevação de custos operacionais
* comprometimento dos indicadores de SST

O SafeVision AI propõe uma abordagem baseada em monitoramento contínuo, prevenção inteligente e tomada de decisão orientada por dados.

---

# Objetivo Geral

Desenvolver uma solução inteligente de segurança industrial capaz de automatizar o monitoramento de EPIs e detectar riscos operacionais em tempo real através de Inteligência Artificial e Visão Computacional.

---

# Objetivos Específicos

* Automatizar o processo de fiscalização operacional
* Detectar ausência de EPIs em tempo real
* Identificar riscos ergonômicos durante movimentação de carga
* Emitir alertas instantâneos para supervisores
* Consolidar indicadores de conformidade operacional
* Criar histórico rastreável de ocorrências
* Apoiar tomada de decisão estratégica
* Reduzir acidentes industriais
* Melhorar indicadores de SST
* Promover cultura de segurança preventiva

---

# Escopo do Projeto

## Dentro do Escopo

* monitoramento contínuo de EPIs
* análise de conformidade operacional
* detecção de postura inadequada
* análise de movimentação industrial
* alertas operacionais em tempo real
* dashboard gerencial
* relatórios analíticos
* armazenamento histórico
* classificação de níveis de risco
* monitoramento por câmeras industriais

## Fora do Escopo

* diagnósticos médicos
* reconhecimento facial biométrico
* integração com folha de pagamento
* controle de recursos humanos
* desenvolvimento de hardware
* monitoramento externo à planta industrial
* alarmes sonoros industriais
* automação física de máquinas

---

# Fluxos Implementados no Protótipo

## Dashboard de Monitoramento

Permite ao supervisor acompanhar:

* indicadores de segurança
* alertas ativos
* status operacional
* conformidade dos colaboradores
* métricas em tempo real

## Gestão de EPIs

Fluxo completo de:

* cadastro de colaborador
* consulta de EPIs
* vinculação de equipamentos
* atualização de registros
* acompanhamento de conformidade

## Alertas e Notificações

Permite:

* visualização de alertas críticos
* histórico de ocorrências
* classificação por criticidade
* acompanhamento de riscos operacionais

## Relatórios de Conformidade

Permite:

* geração de relatórios por setor
* análise de conformidade
* histórico de ocorrências
* indicadores de desempenho em SST

---

# Decisões de UX/UI

O design foi desenvolvido considerando o ambiente industrial e as personas identificadas na Sprint 1.

## Princípios de Design

### Leitura Rápida

* uso de dashboards visuais
* indicadores destacados
* alertas coloridos por criticidade
* informações priorizadas por importância

### Navegação Simplificada

Menu lateral persistente com acesso rápido aos módulos:

* Dashboard
* EPIs
* Alertas
* Relatórios
* Configurações

### Hierarquia Visual

* destaque para eventos críticos
* gráficos operacionais
* métricas de conformidade
* acompanhamento em tempo real

### Contexto Industrial

A interface foi pensada para:

* supervisores industriais
* acompanhamento contínuo
* leitura rápida
* tomada de decisão operacional

---

# Mapeamento entre Casos de Uso e Telas

| Caso de Uso           | Tela           |
| --------------------- | -------------- |
| Consultar Dashboard   | Dashboard      |
| Monitorar Indicadores | Dashboard      |
| Gerenciar EPIs        | Gestão de EPIs |
| Consultar Colaborador | Gestão de EPIs |
| Receber Alertas       | Alertas        |
| Consultar Ocorrências | Alertas        |
| Gerar Relatórios      | Relatórios     |
| Consultar Histórico   | Relatórios     |

---

# Navegação do Protótipo

Fluxo recomendado:

1. Dashboard
2. Gestão de EPIs
3. Consulta de colaboradores
4. Alertas
5. Ocorrências registradas
6. Relatórios
7. Geração de relatório
8. Retorno ao Dashboard

---

# Arquitetura da Solução

## Fluxo Operacional

```text
[Câmeras Industriais]
            ↓
[Captura Contínua de Vídeo]
            ↓
[Processamento Computacional]
            ↓
[YOLO26 + OpenCV]
            ↓
[Motor de Regras]
            ↓
[Classificação de Risco]
            ↓
[API de Processamento]
            ↓
[Banco de Dados]
            ↓
[Dashboard Operacional]
            ↓
[Supervisor Industrial]
```

---

# Tecnologias Selecionadas

| Tecnologia | Aplicação                 |
| ---------- | ------------------------- |
| Python     | Inteligência Artificial   |
| YOLO26     | Detecção de objetos       |
| OpenCV     | Processamento de imagem   |
| FastAPI    | Backend                   |
| PostgreSQL | Banco de dados            |
| React      | Frontend                  |
| TypeScript | Estruturação da aplicação |
| WebSockets | Comunicação em tempo real |

---

# Funcionalidades Principais

* monitoramento contínuo de EPIs
* detecção automática de irregularidades
* análise ergonômica operacional
* classificação inteligente de risco
* geração de alertas críticos
* dashboards operacionais
* relatórios analíticos
* rastreabilidade de conformidade
* histórico de eventos críticos
* consolidação de indicadores industriais

---

# Estrutura da Documentação

## Levantamento de Requisitos

* docs/levantamento-requisitos.md

## Personas

* docs/personas.md

## Regras de Negócio

* docs/regras-de-negocio.md

## Arquitetura da Solução

* docs/arquitetura-da-solucao.md

## Fluxo Operacional

* docs/fluxo-operacional.md

## Análise de Riscos

* docs/analise-de-riscos.md

---

# Diagramas UML

## Casos de Uso

* docs/diagramas/casos-de-uso.md

## Atividades

* docs/diagramas/atividades.md

## Classes

* docs/diagramas/classes.md

## Arquitetura

* docs/diagramas/arquitetura.md

## Entidade Relacionamento

* docs/diagramas/entidade-relacionamento.md

---

# Evidências da Sprint 2

Entregáveis produzidos:

* protótipo navegável no Figma
* MVP funcional em código
* vídeo de apresentação
* documentação UX/UI
* mapeamento de casos de uso
* validação dos fluxos da Sprint 1
* simulação da experiência do usuário

---

# Resultados Esperados

* redução de acidentes operacionais
* redução de afastamentos ergonômicos
* melhoria dos indicadores de SST
* fortalecimento da cultura preventiva
* aumento da produtividade
* maior rastreabilidade industrial
* tomada de decisão orientada por dados

---

# Status do Projeto

✅ Sprint 1 — Engenharia, arquitetura e modelagem documental concluída

✅ Sprint 2 — Prototipação funcional e navegável concluída

### Entregáveis concluídos

* documentação de requisitos
* regras de negócio
* personas
* arquitetura da solução
* diagramas UML
* protótipo navegável
* MVP funcional
* vídeo demonstrativo
* documentação UX/UI

🚀 Próxima etapa: evolução da implementação técnica da solução e validação dos componentes de Inteligência Artificial.
