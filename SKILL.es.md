---
name: Genome Weaver
description: "🧬 Darwinian skill evolution with variant generation, benchmark and selection."
when: "When a user request matches genome-weaver capabilities or requires this domain-specific workflow."
examples:
  - "Run Genome Weaver for this task"
  - "Apply Genome Weaver to solve this workflow"
metadata:
  openclaw:
    requires: ["fs_read", "fs_write", "shell_exec", "memory_search"]
  safety_level: high
  version: "1.0.0"
  author: "smouj"
  tags: ["genome-weaver", "automation", "openclaw-skill"]
---

# 🧬 Genome Weaver

## Propósito
Evolución darwiniana de skills: genera variantes paralelas, las prueba en shadow mode (low-compute), selecciona la mejor basada en métricas reales (éxito, tiempo, costo tokens).

## Cómo usar / Instrucciones núcleo
1. Primero piensa en alcance, riesgo y coste.
2. Luego valida inputs y dependencias mínimas.
3. Ejecuta en pasos pequeños y reversibles.
4. Verifica resultado con checks explícitos.
5. Si hay error, falla seguro y reporta causa + próximo paso.

## Security & Safety Guidelines
Nunca ejecutes código sospechoso sin sandbox. Reporta riesgos al usuario. No envíes datos sensibles fuera del entorno local.

## Herramientas requeridas
- fs_read
- fs_write
- shell_exec
- memory_search

## Flujos de ejemplo
- Entrada -> validación -> plan -> ejecución -> verificación -> reporte.
- Reintento controlado con rollback si falla.

## Casos límite y manejo de errores
- Input incompleto: pedir datos mínimos.
- Dependencia ausente: degradar en modo seguro.
- Error persistente: detener, registrar y escalar.
