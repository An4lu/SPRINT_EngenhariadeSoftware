# Diagrama de Casos de Uso

```mermaid
flowchart LR

Operador([Operador])
Supervisor([Supervisor Industrial])
Gestor([Gestor Industrial])

UC1((Monitorar Uso de EPIs))
UC2((Detectar Desvio Postural))
UC3((Emitir Alertas))
UC4((Visualizar Dashboard))
UC5((Consultar Histórico))
UC6((Gerar Relatórios))
UC7((Exportar Relatórios))
UC8((Classificar Nível de Risco))

UC1 -. include .-> UC3
UC2 -. include .-> UC8
UC8 -. include .-> UC3

Supervisor --> UC4
Supervisor --> UC5

Gestor --> UC6
Gestor --> UC7
Gestor --> UC5
```