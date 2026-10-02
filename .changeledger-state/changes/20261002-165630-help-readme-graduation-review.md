---
id: "20261002-165630"
title: Ayuda del CLI y README con el rol graduation-review
type: quick
status: draft
created: 2026-10-02T16:56:30Z
depends_on: []
related_to: ["20261002-152555"]
owner: Carlos Rodríguez
release_impact: patch
---

## Request

`#20261002-152555` añadió el rol `graduation-review`, pero dos textos escritos a
mano siguen listando sólo cuatro roles:

- en `bin/changeledger.mjs`, la ayuda de `agent-prompt` (sus ejemplos) y la
  descripción de `[change-id]` de `agent-context` («optional for investigation;
  required for implementation, review and post-review»);
- `README.md`: «Roles are `investigation`, `implementation`, `review` and
  `post-review`.».

Añadir `graduation-review` en esos tres sitios, con una frase breve que diga que
es la revisión de solo lectura de la reconciliación de specs de un change
`done`. Si algún test fija esos textos, ajustarlo. Fuera de alcance: el
contrato, las specs y cualquier comportamiento. Se revierte con el commit.

## Log
