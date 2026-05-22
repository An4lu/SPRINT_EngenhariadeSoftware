# Diagrama Entidade Relacionamento

# Objetivo

O Diagrama Entidade Relacionamento representa a estrutura lógica do banco de dados da solução SafeVision AI.

A modelagem foi projetada para garantir:

- rastreabilidade operacional
- integridade de dados
- armazenamento histórico
- suporte analítico
- consolidação de indicadores

---

# Diagrama ER

```mermaid
erDiagram

SETOR ||--o{ OPERADOR : possui
SETOR ||--o{ CAMERA : monitora
OPERADOR ||--o{ DETECCAO_EPI : gera
OPERADOR ||--o{ EVENTO_RISCO : possui
TIPO_EPI ||--o{ DETECCAO_EPI : referencia
EVENTO_RISCO ||--o{ RELATORIO : compoe
RELATORIO ||--o{ INDICADOR : consolida

SETOR {
  int id
  string nome
  string localizacao
  string nivel_risco
}

OPERADOR {
  int id
  string nome
  string matricula
  string cargo
  string status
}

CAMERA {
  int id
  string identificacao
  string localizacao
  string status
}

TIPO_EPI {
  int id
  string nome
  string categoria
  boolean obrigatorio
}

DETECCAO_EPI {
  int id
  boolean detectado
  float confianca
  datetime timestamp
}

EVENTO_RISCO {
  int id
  string tipo_evento
  string nivel_risco
  datetime timestamp
}

RELATORIO {
  int id
  string tipo
  datetime data_geracao
}

INDICADOR {
  int id
  string nome
  float valor
}
```

---

# Objetivos da Modelagem

- garantir rastreabilidade industrial
- consolidar eventos históricos
- suportar dashboards operacionais
- permitir geração de relatórios
- armazenar conformidade operacional
- apoiar análise estratégica