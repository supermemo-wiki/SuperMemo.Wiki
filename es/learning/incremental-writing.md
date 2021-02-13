---
title: Lectura Incremental
description: 
published: true
date: 2021-02-13T17:24:15.530Z
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
  step1{{"New article (next repetition)"}}:::state
  
  subgraph IR[" "]
    IR-step1["Do Incremental Reading"]:::type
    IR-step2>"Read article"]
    IR-step3("<img src='/supermemo/incremental-reading/ir-1st-rep-step-1.png'; width='250px' height='154px'/>")
    IR-step4["Acquire knowledge"]
  end
  
  subgraph IW[" "]
    IW-step1["Do Incremental Writing"]:::type
    IW-step2-a["Update content using new knowledge"]
    IW-step2-b["Add new content"]
    IW-step3["Consolidate knowledge"]
  end
  
  
  step1                   -. If writing article                 -..-> IW-step1
  IW-step1                -- 1.a. Read and locate mistakes        --> IW-step2-a
  IW-step1                -- 1.b. New ideas                       --> IW-step2-b
  IW-step2-a & IW-step2-b                                         --> IW-step3
  IW-step3                -- 2. Repeat until bored                --> IW-step1
  IW-step3                -. 3. When bored with current article   .-> step1
  
  
  step1                   -. If learning article                       -.-> IR-step1
  IR-step1                                                              --> IR-step2
  IR-step2                -- 1. Locate interesting information          --> IR-step3
  IR-step3                -- 2. Extract valuable text for later         --> IR-step4
  IR-step4                -- 3. Repeat until bored with current article --> IR-step2
  IR-step4                -. 4. When bored with current article         .-> step1
  
  classDef state fill:#F3FFDA,stroke-width:2px
  classDef type fill:#72F87C,color:#333
```


## Beneficios

Un escritor incremental típico:

- Nunca te aburres (siempre hay ideas nuevas y variadas para mantener las cosas emocionantes),
- Aumenta tu creatividad (flujo constantemente de nueva información),
- Escribes de manera más eficiente (progresando en varias secciones en paralelo),
- Es menos propenso a errores (dividir en secciones más pequeñas facilita la detección de errores y la actualización de información errónea u obsoleta con nuevos conocimientos).
