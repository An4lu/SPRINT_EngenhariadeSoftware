# Arquitetura da Solução

```text
[Câmeras Industriais]
            ↓
[Visão Computacional]
            ↓
[YOLO26 + OpenCV]
            ↓
[Motor de Regras]
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

# Componentes Principais

## Câmeras Industriais

Responsáveis pela captura contínua do fluxo de vídeo operacional.

## Visão Computacional

Responsável pelo processamento das imagens capturadas.

## YOLO26

Responsável pela inferência computacional e detecção dos EPIs.

## Motor de Regras

Responsável pela validação das regras operacionais e classificação de riscos.

## API de Processamento

Responsável pela comunicação entre os módulos da solução.

## Banco de Dados

Responsável pelo armazenamento histórico e rastreabilidade industrial.

## Dashboard Operacional

Responsável pela visualização em tempo real das ocorrências e indicadores.