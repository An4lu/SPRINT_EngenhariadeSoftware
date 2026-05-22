# Diagrama de Classes

# Objetivo

O Diagrama de Classes representa a estrutura lógica da solução SafeVision AI, modelando as principais entidades do domínio industrial e seus relacionamentos.

A modelagem foi construída considerando:

- rastreabilidade operacional
- monitoramento contínuo
- gestão de conformidade
- análise de risco
- geração de indicadores industriais

---

# Principais Entidades

## Operador

Representa os trabalhadores monitorados pela solução.

---

## Setor

Representa áreas operacionais da planta industrial.

---

## Camera

Representa os dispositivos responsáveis pela captura do fluxo de vídeo.

---

## TipoEPI

Representa os equipamentos de proteção monitorados.

---

## DeteccaoEPI

Representa as inferências computacionais realizadas pelo sistema.

---

## EventoRisco

Representa ocorrências críticas identificadas pela IA.

---

## Dashboard

Representa a visualização operacional em tempo real.

---

## Relatorio

Representa consolidações analíticas e gerenciais.

---

## Indicador

Representa métricas operacionais de conformidade e segurança.

---

# Diagrama UML

```mermaid
classDiagram

class Operador {
  +id
  +nome
  +matricula
  +cargo
  +status
  +setor
}

class Setor {
  +id
  +nome
  +nivelRisco
  +localizacao
}

class Camera {
  +id
  +identificacao
  +localizacao
  +status
  +anguloCaptura
}

class TipoEPI {
  +id
  +nome
  +categoria
  +obrigatorio
}

class DeteccaoEPI {
  +id
  +confianca
  +detectado
  +timestamp
  +frameReferencia
}

class EventoRisco {
  +id
  +tipoEvento
  +nivelRisco
  +descricao
  +timestamp
  +statusEvento
}

class Dashboard {
  +id
  +tipoVisualizacao
  +ultimaAtualizacao
}

class Relatorio {
  +id
  +tipo
  +periodo
  +dataGeracao
}

class Indicador {
  +id
  +nome
  +valor
  +periodo
}

Setor "1" --> "N" Operador
Setor "1" --> "N" Camera
Operador "1" --> "N" DeteccaoEPI
Operador "1" --> "N" EventoRisco
TipoEPI "1" --> "N" DeteccaoEPI
EventoRisco "1" --> "N" Relatorio
Dashboard --> Indicador
Relatorio --> Indicador
```

---

# Relacionamentos Principais

| Relacionamento | Descrição |
|---|---|
| Setor → Operador | Um setor possui múltiplos operadores |
| Setor → Camera | Um setor pode possuir múltiplas câmeras |
| Operador → DeteccaoEPI | Um operador pode gerar múltiplas detecções |
| Operador → EventoRisco | Um operador pode possuir múltiplos eventos |
| TipoEPI → DeteccaoEPI | Um EPI pode estar relacionado a diversas detecções |
| EventoRisco → Relatorio | Eventos compõem relatórios analíticos |