# Contribuir a raxar-solutions

> Este es el documento canonical de proceso. Cada repo enlaza aquí para
> evitar drift entre copias.

## Requisitos previos

- Pertenecer al GitHub org `raxar-solutions` o ser invitado a un repo concreto
- 2FA habilitado (TOTP mínimo · YubiKey recomendado para producción)
- Acceso a los canales operativos (Telegram supergroup `RAXAR Command Center`)

## Flujo de trabajo (PR-based)

1. **Issue primero** · abre o referencia un issue antes de empezar trabajo no trivial.
   - Bug → `[bug]` template
   - Feature → `[feat]` template (incluye criterios de aceptación)
   - Pregunta → `[?]` template
2. **Branch desde `main`** · nombre `<tipo>/<scope>-<short-desc>` (ej. `feat/dashboard-llm-router-v3`)
3. **Atomic commits** · Conventional Commits (`feat:`, `fix:`, `docs:`, `chore:`, `refactor:`, `test:`, `ci:`, `perf:`, `security:`)
4. **PR contra `main`** · usa el template · vincula el issue (`Closes #N`)
5. **CI verde obligatorio** · vitest/pytest + tsc + lint + n8n compliance (donde aplique)
6. **≥1 review aprobada** del CODEOWNERS correspondiente
7. **Squash merge** (linear history enforced por ruleset)
8. **Cleanup** · elimina la rama tras merge

## Estilo de código

- TypeScript: strict mode · 0 errors antes de PR
- Python: ruff + mypy (donde configurado)
- Tests para todo cambio de comportamiento (TDD recomendado · ver `superpowers:test-driven-development`)
- Sin secretos en commits · `.env*` siempre gitignored
- LLM Router obligatorio para llamadas a modelos (no APIs directas · ver CLAUDE.md §6.5)

## Hard gates pre-merge

- [ ] CI verde
- [ ] CODEOWNERS aprobado
- [ ] Sin secretos / PII / credenciales
- [ ] Workflow compliance preserved (n8n: errorWorkflow + executionTimeout)
- [ ] RLS preservado (`fenix.*` tablas)
- [ ] Multi-tenant: `tenant_id` propagado

## Decisiones arquitectónicas (ADRs)

Cualquier cambio que afecte:
- Estructura de packages / repos
- Schema DB (`fenix.*`)
- Flujo de autenticación
- LLM Router / cost guardrails
- Infra crítica (Coolify · Traefik · Tailscale)

requiere un ADR previo en `raxar-docs/KNOWLEDGE/architecture/ADRs/` referenciado
desde el PR. Sin ADR aprobado → bloqueado.

## Documentación canónica

- `raxar-docs/CLAUDE.md` — memoria operativa del IT Agent senior
- `raxar-docs/KNOWLEDGE/architecture/` — patrones · ADRs · referencias
- `raxar-docs/KNOWLEDGE/onboarding/` — guías para nuevos miembros
- `raxar-docs/INFRA/RUNBOOKS/` — operaciones · incident response · deploys

## Soporte

- Telegram supergroup · topic correspondiente al área (#dev · #infra · #ops)
- Email `team@raxar.es` para asuntos privados

---

*Última actualización: 2026-05-04 · S267.3*
