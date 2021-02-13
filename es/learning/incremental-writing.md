---
title: Lectura Incremental
description: 
published: true
date: 2021-02-13T17:36:57.171Z
tags: 
editor: markdown
dateCreated: 2021-02-13T17:17:10.364Z
---

# Escritura incremental

**Escritura incremental(EI)** es un método para impulsar la creatividad, la calidad y el placer de escribir. Se sinergiza con la capacidad natural de tu cerebro para actualizar el conocimiento y organizarlo en redes de conceptos.

La escritura incremental es una extensión de [lectura incremental](/learning/incremental-reading). Deberías estar familiarizado con ello antes de considerar la escritura incremental.

## ¿Como funciona?

La escritura incremental suele contar con la asistencia de un software para maximizar el uso de tu tiempo intercalando:

- Revisar nuevo material de aprendizaje para desarrollar nuevos conocimientos,
- Revisar los conocimientos adquiridos previamente para conservarlos en el tiempo (¡para siempre!),
- Trabajo creativo (redacción, resolución de problemas, etc).

En LI, la decisión de si debes continuar trabajando en un texto en particular depende de tu deseo de hacerlo. Ese deseo es un compuesto de variables: [placer de escribir](/reference-manual/pleasure-of-learning), estado de fluidez, nivel de comprensión del tema, etc.


```mermaid

graph TB
  paso1{{"Artícluo nuevo (próxima repetición)"}}:::state
  
  subgraph LI[" "]
    LI-paso1["Leer incrementalmente"]:::type
    LI-paso2>"Leer el artículo"]
    LI-paso3("Aprendizaje no asociativo")
    LI-paso4["Adquirir conocimiento"]
  end
  
  subgraph EI[" "]
    EI-paso1["Escribir incrementalmente"]:::type
    EI-paso2-a["Actualizar contenido usando el nuevo conocimiento"]
    EI-paso2-b["Añadir nuevo contenido"]
    EI-paso3["Consolidar nuevo conocimiento"]
  end
  
  
  paso1                   -. Si escribiendo artículo                 -..-> EI-paso1
  EI-paso1                -- 1.a. Lee y localiza errores        --> EI-paso2-a
  EI-paso1                -- 1.b. Nuevas ideas                       --> EI-paso2-b
  EI-paso2-a & EI-paso2-b                                         --> EI-paso3
  EI-paso3                -- 2. Repetir hasta sadisfacerse               --> EI-paso1
  EI-paso3                -. 3. Cuando te aburras del artículo actual   .-> paso1
  
  
  paso1                   -. Si leyendo artículo                       -.-> LI-paso1
  LI-paso1                                                              --> LI-paso2
  LI-paso2                -- 1. Localiza información interesante          --> LI-paso3
  LI-paso3                -- 2. Extrae texto valioso para más adelante         --> LI-paso4
  LI-paso4                -- 3. Repite hasta que te aburra el artículo actual --> LI-paso2
  LI-paso4                -. 4. Cuando te aburra el artículo actual         .-> paso1
  
  classDef state fill:#F3FFDA,stroke-width:2px
  classDef type fill:#72F87C,color:#333
```



## Beneficios

Un escritor incremental típico:

- Nunca te aburres (siempre hay ideas nuevas y variadas para mantener las cosas emocionantes),
- Aumenta tu creatividad (flujo constantemente de nueva información),
- Escribes de manera más eficiente (progresando en varias secciones en paralelo),
- Es menos propenso a errores (dividir en secciones más pequeñas facilita la detección de errores y la actualización de información errónea u obsoleta con nuevos conocimientos).
