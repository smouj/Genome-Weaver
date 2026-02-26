---
name: genome-weaver
description: "🧬 Evolución darwiniana de skills."
metadata:
  {
    "openclaw": {
      "emoji": "🧬",
      "version": "0.2.0",
      "author": "smouj",
      "lang_default": "en"
    }
  }
---

# 🧬 Genome Weaver

## Propósito
Motor evolutivo que genera variantes de skills, ejecuta pruebas A/B, mide desempeño y selecciona la configuración más efectiva según éxito, coste y latencia.

## Tags
- security
- reliability
- automation
- openclaw-skill

## Contrato de ejecución
1. Validar solicitud y restricciones.
2. Generar plan mínimo seguro.
3. Ejecutar en pasos reversibles.
4. Verificar con checks explícitos.
5. Resumir resultado + siguientes acciones.

## Inputs esperados
- Objetivo
- Restricciones (tiempo/coste/privacidad)
- Archivos/URLs opcionales

## Outputs
- Plan
- Acciones ejecutadas
- Verificación
- Notas de rollback

## Guardrails
- Nunca exponer secretos.
- Sin acciones destructivas sin confirmación explícita.
- Fallar de forma segura con diagnóstico accionable.

## Comandos
```bash
printf "genome-weaver: validar -> ejecutar -> verificar\n"
```

## Checklist de test
- [ ] Happy path
- [ ] Manejo de errores
- [ ] Idempotencia
- [ ] Guardrails respetados
