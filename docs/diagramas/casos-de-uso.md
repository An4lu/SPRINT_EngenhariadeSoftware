# Diagrama de Casos de Uso

```mermaid
flowchart LR

Operador([Operador Industrial])
Supervisor([Supervisor de Segurança])
Gestor([Gestor Industrial])
Sistema([Sistema SafeVision AI])

UC1((Monitorar Operadores))
UC2((Detectar Uso de EPIs))
UC3((Detectar Desvio Postural))
UC4((Classificar Risco))
UC5((Emitir Alertas))
UC6((Atualizar Dashboard))
UC7((Consultar Histórico))
UC8((Gerar Relatórios))
UC9((Exportar Relatórios))
UC10((Consolidar Indicadores))
UC11((Registrar Eventos))

Sistema --> UC1
Sistema --> UC2
Sistema --> UC3
Sistema --> UC4
Sistema --> UC5
Sistema --> UC11

UC2 -. include .-> UC4
UC3 -. include .-> UC4
UC4 -. include .-> UC5
UC5 -. include .-> UC6
UC11 -. include .-> UC7

Supervisor --> UC6
Supervisor --> UC7

Gestor --> UC8
Gestor --> UC9
Gestor --> UC10
Gestor --> UC7
```