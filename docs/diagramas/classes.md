# Diagrama de Classes

```mermaid
classDiagram

class Operador {
  +id
  +nome
  +cargo
  +matricula
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
  +obrigatorio
  +categoria
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
  +periodo
  +tipo
  +dataGeracao
}

class Indicador {
  +id
  +nome
  +valor
  +periodo
}

Setor --> Operador
Setor --> Camera
Operador --> DeteccaoEPI
Operador --> EventoRisco
TipoEPI --> DeteccaoEPI
EventoRisco --> Relatorio
Dashboard --> Indicador
Relatorio --> Indicador
```