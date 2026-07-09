# Uso seguro de IA en auditorías internas

## Principio

La IA puede apoyar análisis, redacción y organización de información, pero no debe reemplazar el juicio auditor ni la revisión de evidencias.

## Información que no debe cargarse en herramientas no autorizadas

- Bases completas con datos personales de afiliados, beneficiarios, trabajadores o usuarios.
- Documentos con números de identificación, historia laboral, datos de salud, dirección, teléfono o información financiera identificable.
- Contraseñas, tokens, credenciales, archivos `.env`, logs sensibles o accesos internos.
- Expedientes completos si no han sido anonimizados.
- Información jurídica sensible sin autorización.

## Buenas prácticas

- Anonimizar muestras cuando sea posible.
- Usar códigos de caso en lugar de nombres o cédulas.
- Compartir solo campos necesarios para el análisis.
- Validar la respuesta de la IA contra los documentos reales.
- No copiar conclusiones sin revisión del auditor.
- No pedir a la IA que invente fuentes, normas o evidencias.
- Conservar el criterio institucional y el formato aprobado.

## Prompt de seguridad

```text
Analiza esta información como apoyo a auditoría interna. No infieras datos personales ni generes conclusiones que no estén soportadas. Si falta evidencia, marca `por verificar`. No solicites ni expongas datos sensibles innecesarios. Entrega solo análisis útil para el auditor.
```

## Señales de alerta en una respuesta de IA

- Afirma cumplimiento sin evidencia.
- Cita normas o requisitos no entregados.
- Recomienda acciones genéricas.
- Confunde observación con no conformidad.
- Genera datos, fechas o responsables que no estaban en los documentos.
- Propone más formatos sin justificar el valor.
