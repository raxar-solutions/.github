<!--
  PR template · raxar-solutions
  Borra secciones que no apliquen · sé específico (lo lee humano + Claude review)
-->

## Resumen
<!-- 1-2 frases · qué cambia · por qué -->

## Cross-references
<!-- Sesión GSD (S###) · ADR · spec · issue · runbook · roadmap -->

- ADR / spec:
- Issue / sesión:

## Tipo de cambio
- [ ] feat (funcionalidad nueva)
- [ ] fix (bugfix)
- [ ] refactor (sin cambio funcional)
- [ ] docs (documentación)
- [ ] chore (build · deps · tooling)
- [ ] ci (workflows · automation)
- [ ] test (añadir/refactor tests)
- [ ] perf (performance)
- [ ] security (hardening · vulnerabilidad)

## Cómo se ha probado
<!-- Tests añadidos · smoke E2E · curls · screenshots si UI -->

- [ ] Vitest / pytest pass local
- [ ] TypeScript strict 0 errors (si aplica)
- [ ] Build verified (si aplica)
- [ ] Smoke prod / staging (si aplica · indicar URL)

## Compliance · checklist hard gates
- [ ] Sin secretos comiteados (verificado `git diff` · `.env*` ignorados)
- [ ] RLS preservado si toca tablas (`fenix.*`)
- [ ] Workflow compliance preserved si toca n8n (errorWorkflow + executionTimeout)
- [ ] LLM Router usado si llamadas LLM nuevas (no APIs directas)
- [ ] PII redactada si toca pipelines de IA pública
- [ ] Tenant_id propagado si toca queries multi-tenant
- [ ] HMAC en webhooks públicos nuevos
- [ ] Sin breaking changes en APIs externas (o documentadas)

## Riesgo / blast radius
- [ ] 🟢 Bajo · feature aislada · rollback rápido
- [ ] 🟡 Medio · toca pipeline activa · rollback con plan
- [ ] 🔴 Alto · destructivo · spec required + ADR

## Plan de rollback
<!-- Cómo revertir si algo falla en prod · tag previo · script · manual -->

## Notas para reviewer
<!-- Cosas que necesitas que mire · áreas no triviales · decisiones implícitas -->
