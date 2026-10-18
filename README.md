# Arquitecto-banca-internet-BP
Ejercicio práctico de arquitectura de soluciones con modelo C4
***Autor:** Diego Gerardo Zamora Cruz
***Fecha:** octubre de 2026

## Contenido
-[Documento de arquitectura (PDF)](Arquitectura-Banca-por-Internet-diza.pdf)
-[Diagramas fuente (draw.io)]
## Resumen

- SPA en React y app móvil en Flutter, cada una con su BFF.
- Autenticación con OAuth 2.0 / OIDC: Authorization Code con PKCE, passkeys y MFA para operaciones sensibles.
- Microservicios en Amazon ECS Fargate detrás de un API Gateway, con saga, outbox e idempotencia para las transferencias.
- Notificaciones y auditoría desacopladas por eventos.
- AWS en dos regiones (warm standby) con Direct Connect redundante hacia el centro de datos de BP.
