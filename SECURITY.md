# Política de seguridad · raxar-solutions

## Reportar una vulnerabilidad

Si descubres una vulnerabilidad en cualquier sistema RAXAR (servicios públicos
en `raxar.es`, APIs, dashboard, agentes IA, infraestructura), **NO abras un
issue público**. Repórtala de forma privada:

- **Email**: `security@raxar.es` (cifrado opcional vía PGP — solicita la clave en el primer mensaje)
- **Tiempo de respuesta**: ≤ 48h para acuse de recibo · ≤ 7 días para diagnóstico inicial

## Qué incluir

- Descripción del problema y por qué es explotable
- Pasos de reproducción (PoC mínimo)
- Versión / commit / URL afectada
- Impacto estimado y blast radius
- Tu nombre / handle si quieres ser acreditado en el agradecimiento público

## Qué esperar de nosotros

- Acuse de recibo en ≤ 48h
- Validación + plan de mitigación en ≤ 7 días
- Coordinación de disclosure responsable contigo
- Crédito público (con tu permiso) en `KNOWLEDGE/security/HALL_OF_FAME.md`

## Alcance

✅ **Dentro de scope**:
- `*.raxar.es` y `*.aurenix.cloud` (dominio dual transicional)
- Repos públicos en `raxar-solutions/`
- APIs documentadas en `KNOWLEDGE/architecture/`

❌ **Fuera de scope**:
- DoS / volumetric attacks (no autorizados)
- Ingeniería social / phishing al equipo
- Sistemas de partners no operados por RAXAR
- Vulnerabilidades en software de terceros sin impacto demostrable en RAXAR

## Reconocimientos

Mantenemos un Hall of Fame en `KNOWLEDGE/security/HALL_OF_FAME.md` con los
investigadores que han ayudado a hacer RAXAR más seguro.

---

*Última actualización: 2026-05-04 · S267.3*
