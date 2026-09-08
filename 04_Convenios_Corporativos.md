# Convenios Corporativos — Aktiva-T / CEB

**Modelo maestro vigente:** `Convenio_Aktiva-T_Club_Leones_Patagonia.pdf` (esta misma carpeta) — confirmado por Edgar el 20-07-2026 como plantilla de referencia para todos los convenios nuevos.

El convenio con Tropera (`Convenios\Convenio_Tropera_AktivaT.pdf`, junio 2026) queda como antecedente histórico — usaba un modelo más simple (solo Studio, 30% plano) que ya no es el que se ofrece.

## Modelo general del convenio (Club Leones de la Patagonia)

Convenio formal entre el Ecosistema Aktiva-T y una organización (empresa, club deportivo, institución), con:
- **Descuento independiente por unidad** — no un porcentaje único para todo el ecosistema.
- Cobertura de **las unidades activas**: Box, Studio, Cafetería (una organización puede incluir todas o solo algunas). **Clínica Aktiva-T ya no forma parte del ecosistema activo — no incluirla en convenios nuevos.**
- Mecanismo **"Pase Aktiva-T"**: plan activo en gym (Box o Studio) activa automáticamente el descuento en Cafetería. Si el plan de gym vence, el descuento en cafetería se suspende solo.
- Beneficio activado mediante **credencial de la organización vigente** (o "Pase Aktiva-T" en el caso de cafetería).

### Ejemplo aplicado (caso Club Leones de la Patagonia)
**Nota:** la fila de Clínica queda como registro histórico de lo firmado en el PDF original — el beneficio ya no aplica porque la Clínica salió del ecosistema activo (ver [01_Ecosistema_y_Ubicaciones.md](01_Ecosistema_y_Ubicaciones.md)). No usar esta fila para responder consultas actuales de convenio.

| Servicio | Descuento | Dirección | Condición |
|---|---|---|---|
| Box Aktiva-T | 15% en membresía mensual | Barroso 777 | Credencial vigente |
| Studio Aktiva-T (CEB) | 10% en membresía mensual | Baquedano 872 | Credencial vigente |
| Cafetería Aktiva | 5% en consumo diario | Baquedano 872 | Pase Aktiva-T activo |
| ~~Clínica Aktiva-T~~ | ~~5% en 1ª consulta (Med. General, Traumatología, Nutricionista)~~ | Colón 203 | **Inactivo — Clínica fuera del ecosistema** |

### Tabla de precios con descuento — Box (15%)
| Plan | Precio oficial | Precio convenio | Ahorro |
|---|---|---|---|
| Plan Inicia (8 ses.) | $45.000 | $38.250 | −$6.750 |
| Plan Aktivo (10 ses.) | $59.000* | $50.150* | −$8.850* |
| Plan Open Box (ilimitado) | $75.000 | $63.750 | −$11.250 |

\* El PDF original del convenio traía el Plan Aktivo en $56.000 con precio convenio $47.600 — **desactualizado**. Edgar confirmó el 20-07-2026 que el precio de lista oficial es **$59.000**; la tabla de arriba ya usa el valor corregido.

### Tabla de precios con descuento — Studio (10%)
| Plan | Precio oficial | Precio convenio | Ahorro |
|---|---|---|---|
| Plan Esencial | $105.000 | $94.500 | −$10.500 |
| Plan Pro | $140.000 | $126.000 | −$14.000 |

## Condiciones generales del modelo
- Descuentos de uso **personal e intransferible** para socios/colaboradores activos de la organización.
- Credencial de la organización debe presentarse al contratar el servicio.
- Beneficios **no acumulables** con otras promociones vigentes, salvo indicación expresa.
- Aktiva-T se reserva el derecho de **modificar tarifas base con aviso previo de 30 días** a la organización.
- **Vigencia inicial: 12 meses**, renovable de común acuerdo entre las partes (distinto al modelo Tropera, que usaba 6 meses + revisión a los 3).
- Contacto y firmante: **Fidel Pinilla Andrade**, Director Ecosistema Aktiva-T (fidelpinilla@gmail.com · +56 9 7704 0971).
- El convenio incluye datos formales de la organización beneficiaria: nombre, RUT, dirección, contacto — quedan "por confirmar" si no se tienen al momento de emitir la propuesta.

## Pasos del proceso
1. Recolección de datos de la organización interesada (ver [08_Datos_Convenio_para_Prompt_Akti.md](08_Datos_Convenio_para_Prompt_Akti.md)).
2. Definición de qué unidades incluye y el % de descuento por unidad (caso a caso, no hay un default único obligatorio).
3. Generación de la propuesta en PDF (ver Sistema de Convenios CEB, abajo).
4. Revisión y ajuste de condiciones si corresponde.
5. Firma del convenio.
6. Seguimiento del estado (Prospecto → Propuesta enviada → Firmado → Activo).

## Nota sobre "criterios de convenio institucional"
Los criterios formales para calificar qué organizaciones acceden a convenio, y qué % de descuento corresponde por defecto a cada tipo (empresa vs. club deportivo vs. institución), **no están cerrados aún** — responsable: Fidel (ver [07_Decisiones_y_Pendientes.md](07_Decisiones_y_Pendientes.md)).

## Automatización (desde 20-07-2026)
Sistema de generación automática de propuestas: una hoja de Google Sheets con los datos de cada organización interesada + un botón (Apps Script) que genera el PDF con esta misma estructura (multi-unidad, descuento por servicio, Pase Aktiva-T, condiciones editables).

- Archivos: `Convenios\Sistema de Convenios CEB\` (Excel de datos, Code.gs, plantilla HTML, instrucciones).
- Datos que debe recolectar Akti por WhatsApp antes de derivar: ver [08_Datos_Convenio_para_Prompt_Akti.md](08_Datos_Convenio_para_Prompt_Akti.md).
