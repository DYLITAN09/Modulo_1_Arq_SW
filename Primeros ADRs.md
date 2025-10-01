# ADR 001 – Estilo Arquitectónico

## Contexto
El sistema F-eCX debe ser una plataforma regional que permita interoperabilidad entre países, asegurando integridad y trazabilidad en la emisión y validación de facturas electrónicas de comercio exterior.

## Decisión
Se adopta un **arquitectura basada en microservicios desacoplados**, con integración mediante APIs y eventos (event-driven).

## Justificación
- Escalabilidad: cada módulo (validación, firma digital, intercambio) puede evolucionar de forma independiente.
- Resiliencia: fallos en un microservicio no afectan al resto.
- Facilita la adopción gradual en distintos países.

## Alternativas consideradas
- **Monolito modular:** menor complejidad inicial, pero limitado en escalabilidad regional.
- **SOA tradicional:** demasiado acoplado a buses centralizados (ESB).

## Consecuencias
- Aumento en complejidad de despliegue (requiere CI/CD, observabilidad).
- Mayor necesidad de gobernanza de APIs y contratos de eventos.
---
# ADR 002 – Estrategia de Interoperabilidad

## Contexto
El proyecto RG-T4185 busca que las facturas electrónicas de exportación se conviertan en comprobantes de importación, entre distintas administraciones tributarias y aduaneras.

## Decisión
Usar una **plataforma regional de interoperabilidad basada en estándares internacionales (WCO Data Model, UBL, JSON/Avro)** y **contratos de APIs/eventos versionados**.

## Justificación
- Garantiza interoperabilidad semántica entre países.
- Facilita validación automatizada de comprobantes.
- Adopta lineamientos ya usados en iniciativas multilaterales.

## Alternativas consideradas
- Integración punto a punto entre países (alta complejidad de mantenimiento).
- Uso de formatos propietarios (riesgo de lock-in).

## Consecuencias
- Se requiere gobernanza regional de contratos.
- Necesidad de catálogos de esquemas versionados.
---
# ADR 003 – Enfoque de Firma y Validación

## Contexto
El sistema debe asegurar la autenticidad e integridad de las facturas electrónicas (F-eCX), cumpliendo requisitos regulatorios.

## Decisión
Adoptar **Credenciales Verificables (VCs) e Identificadores Descentralizados (DIDs)** como mecanismo base, con soporte de **PKI tradicional (X.509, OCSP/CRL)** para compatibilidad.

## Justificación
- Cumple con el requisito del BID de usar VCs/DIDs.
- Asegura verificabilidad descentralizada de comprobantes.
- Mantiene compatibilidad con infraestructuras existentes de firma digital.

## Alternativas consideradas
- Uso exclusivo de PKI centralizada (no cumple lineamiento de innovación).
- Uso exclusivo de VCs/DIDs sin PKI (riesgo regulatorio en países que aún exigen PKI).

## Consecuencias
- Complejidad adicional de integrar dos modelos (VCs/DIDs + PKI).
- Necesidad de estandarización en validación transfronteriza.
