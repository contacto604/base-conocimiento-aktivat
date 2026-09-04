# Decisiones y Pendientes — Aktiva-T / CEB

## Decisiones confirmadas por Edgar (17-07-2026)

1. **Dirección del Box:** Almirante Barroso 777, esquina Colón, Coyhaique.
2. **Paquetes de sesiones en UF (precios 2025):** obsoletos para clientes nuevos. Siguen vigentes solo para alumnos antiguos, hasta fin de 2026. Alumnos nuevos van a la lista de precios vigente en CLP (VIP 8, VIP 12, Esencial, Pro, Box).
3. **Congelamiento de planes Esencial/Pro/Box:** procede solo bajo circunstancias específicas, con comprobante médico u otra justificación válida, y siempre documentado. No es autoservicio; recepción deriva a Dirección.

## Decisiones confirmadas por Edgar (20-07-2026)

4. **Modelo maestro de convenios:** el convenio Club Leones de la Patagonia reemplaza al de Tropera como plantilla de referencia para el Sistema de Convenios CEB (multi-unidad, descuento por servicio, Pase Aktiva-T, vigencia 12 meses).
5. **Precio Plan Aktivo de Box:** el PDF del convenio Club Leones traía $56.000 — Edgar confirmó que el precio de lista oficial vigente es **$59.000**. El sistema de convenios y la base de conocimiento ya usan el valor corregido.
6. **Horario real del Box:** el horario documentado antes ("igual todos los días, 08:00–13:00 y 17:00–20:00") no coincidía con la imagen real compartida por Edgar. El horario correcto varía por día — ver [01_Ecosistema_y_Ubicaciones.md](01_Ecosistema_y_Ubicaciones.md). Corregido en la base y en el buscador.
7. **WhatsApp del Box:** +569 73554774 confirmado como el número vigente y actual del Box (distinto del WhatsApp general de CEB, +56942582210 — ambos son canales válidos, cada uno para su unidad).
8. **Plan Pro no incluye seguimiento personalizado:** el Documento Maestro original lo mencionaba para el Plan Pro, pero es un error — ese beneficio es exclusivo del VIP. Corregido en la base de conocimiento, el buscador y la fuente original (`Aktiva-T_Documento_Maestro_Membresias.md`, corregido 23-07-2026).
9. **Módulo Acceso Total:** aclarado que es un adicional exclusivo para quienes ya tienen una membresía VIP contratada — no se vende de forma independiente.

## Pendientes heredados del Documento Maestro (sección 20, aún no cerrados)

| Decisión | Responsable | Urgencia |
|---|---|---|
| Antigüedad mínima exacta para calificar como "alumno antiguo" (descuento 20% / vigencia de paquetes UF) | Fidel | Alta |
| Criterios formales de "convenio institucional" | Fidel | Alta |
| Cantidad de días de bloqueo por inasistencias consecutivas (¿3 o 5?) | Edgar / Fidel | Media |
| Definición concreta de actividades de Comunidad VIP (networking, uso Deco Work, etc.) | Edgar | Media |
| Confirmación de capacidad Pilates personalizado con instructora actual + segunda sede | Edgar | Alta |
| Criterios formales adicionales de congelamiento (más allá de "justificación médica documentada") | Fidel | Media |
| Integración del modelo de convenios corporativos con los descuentos VIP | Edgar | Baja |

## Pendiente resuelto (22-07-2026)

- ~~Discrepancia de precios de sesión suelta/clase de prueba entre el prompt de Akti y el Documento Maestro~~ — **Resuelto por Edgar:** los valores correctos son **$10.000 (entrenamiento asistido)** y **$15.000 (Pilates Reformer grupal)**, como decía el prompt de Akti. El Documento Maestro original (sección 5 y 10, con $12.000/$18.000) queda desactualizado y debe corregirse ahí también.

## Pendiente anotado por Edgar (20-07-2026) — sin resolver aún

- **Convenios de reciprocidad de Aktiva-T con otros negocios (el "Pase Aktiva-T" a la inversa):** falta agregar al prompt de Akti información sobre los convenios que los usuarios/socios de Aktiva-T tienen disponibles en **otros comercios** — ej. CEM, Cafetería (otro distinto a la Cafetería Aktiva propia, a confirmar), Tienda Golden Place, etc. Esto es distinto a los convenios corporativos de la sección 04 (que son para que EMPRESAS traigan a SUS colaboradores a Aktiva-T) — acá es al revés: beneficios que Aktiva-T consiguió para SUS socios en negocios externos. Falta: listado completo de estos convenios, condiciones de cada uno, y cómo debe responderlos Akti cuando un socio pregunte. Responsable: Edgar.

  **Pedido para la landing (23-07-2026):** Edgar pidió agregar una sección visual con los logos de estas empresas aliadas y el beneficio que cada una da a la comunidad Aktiva-T. No implementado aún — **no hay datos reales para construirla** (no se puede inventar nombres de empresas ni condiciones en una página pública). Para activarla, Edgar debe enviar, por cada alianza:
  - Nombre de la empresa/negocio
  - Logo (archivo de imagen, idealmente PNG con fondo transparente)
  - Beneficio exacto para socios Aktiva-T (% descuento, qué servicio, requisito para activarlo — ej. mostrar credencial o Pase Aktiva-T)

  Con esos 3 datos por alianza, la sección se arma en minutos (grilla de logos + beneficio debajo de cada uno, estilo consistente con el resto de la landing).

## Pendiente anotado por Edgar (22-07-2026) — landing page

- **Horarios por actividad:** faltan los horarios reales de cada disciplina (musculación, Indoor Cycling, Pilates Reformer, Cross Training, GAP, Recovery, y las 4 actividades nuevas) para publicarlos en la landing. Hoy la landing deriva esta pregunta a WhatsApp en el FAQ, sin inventar horarios. Ya existen fuentes parciales: `Horarios Indoor Cycling.docx`, `Horarios Pilates Reformer (baquedano).docx`, y el horario del Box en [01_Ecosistema_y_Ubicaciones.md](01_Ecosistema_y_Ubicaciones.md) — falta consolidar todo y confirmar vigencia antes de publicar. Responsable: Edgar.

  **Propuesta de diseño para cuando los horarios estén listos** (sugerida por Claude, a validar): un calendario único en la landing con checkboxes por actividad arriba (Musculación, Cycling, Pilates, Cross Training, GAP, Recovery, etc.) — al marcar uno o varios, el calendario debajo filtra y muestra solo esos bloques horarios, por día de la semana. Evita mostrar 8 tablas separadas (satura) y evita un calendario único abarrotado con todo junto. Requiere los horarios reales consolidados antes de construirse — no se implementa hasta tener esa data.

- ~~Módulo de convenios (empresas/clubes) en la landing~~ — **Resuelto (23-07-2026, backend final 31-07-2026):** agregado punto de entrada "Convenios" en el menú y en el footer, que abre un modal con formulario (nombre de organización, tipo, nombre y cargo de contacto, teléfono, email, N° aproximado de personas interesadas, unidades de interés). Pasó por 3 versiones de backend: WhatsApp → `mailto:` → Netlify Forms → **versión final: Google Apps Script Web App** (ver más abajo, "Registro de leads en Sheets"), que escribe directo en la pestaña "Convenios" de la misma planilla del Sistema de Convenios CEB.

- ~~Registro de leads (Convenios, Solicitud de equipo, Interés general) en Sheets~~ — **Resuelto (31-07-2026):** los 3 formularios de la landing (Convenios, Solicitud de equipo, widget de "Contáctanos"/fuera de horario) apuntan a un único **Google Apps Script Web App** (`WebApp_Leads.gs`, en `Convenios\Sistema de Convenios CEB\`, mismo proyecto de Apps Script que genera los PDF de convenio, archivo separado de `Code.gs`). Cada formulario escribe en su pestaña: Convenios → pestaña "Convenios" existente (solo llena lo que el formulario pregunta; % descuento/precios se llenan a mano al negociar); Solicitud de equipo → pestaña nueva "Solicitud Equipos"; widget → pestaña nueva "Interes Web". Cada envío también manda un correo de aviso a `contacto@aktiva-t.com` vía `MailApp`.
  - Reemplaza Netlify Forms para estos 3 formularios (elegido para evitar el límite de 100 envíos/mes del plan gratuito y tener una base de datos real y filtrable en Sheets, en vez de solo un listado en el dashboard de Netlify).
  - **Bug encontrado y corregido:** `appendRow()` dejaba ~35 filas vacías invisibles antes de escribir el dato nuevo (Sheets a veces "cree" que la última fila con contenido está más abajo de lo real). Se corrigió buscando manualmente la última fila con dato real en la columna A antes de escribir.
  - **Cada vez que se edite el código del script, hay que crear una "Nueva implementación"** (Implementar → Nueva implementación) para que la URL ya conectada a la landing tome los cambios — editar y guardar el código no basta.
  - Verificado extremo a extremo el 31-07-2026: escritura en Sheet ✅ y correo de notificación ✅ en los 3 formularios.

- **Precio de la actividad restante del Box** (Clínica formativa de fútbol): sigue como tarjeta descriptiva en "Las experiencias", sin precio público — la landing dice "consulta valor y horarios" / deriva a WhatsApp. Falta que Edgar confirme precios para publicarlo.

- ~~Widget de captura fuera de horario~~ — **Resuelto (24-07-2026):** el botón flotante de WhatsApp detecta automáticamente (con la hora del navegador de quien visita) si está fuera del horario de recepción de Baquedano (Lun-Vie 06:00-22:00, Sáb 09:00-13:00, domingo cerrado). Fuera de ese horario, el botón cambia de color (gris/apagado), su texto pasa a "Fuera de horario", y en vez de abrir WhatsApp abre un mini-formulario: elige qué le interesa (Studio, Box, Recovery, Coworking, Convenios, Otro con botones tipo chip) + nombre + teléfono, se envía por Netlify Forms (`interes-web`) sin salir de la página, y deja igual la opción de escribir por WhatsApp para quien prefiera ese canal aunque tarde en responder. Reemplaza la idea original de un chatbot de WhatsApp vía Make (Akti sigue existiendo como prompt/automatización en Make, pero está sin saldo/pausada — se optó por esta alternativa sin costo ni dependencia de saldo).
  - **Pendiente de Edgar:** agregar `interes-web` a las notificaciones por correo en el mismo panel de Netlify (Emails and webhooks → Form submission notifications), igual que se hizo con "convenios" y "solicitud-equipo".

- ~~Formulario de solicitud de "Preparación física de equipos"~~ — **Resuelto (24-07-2026):** reemplazado el link de WhatsApp por un modal con formulario propio (`solicitud-equipo`), mismo patrón que Convenios (Netlify Forms, sin backend propio). Campos: nombre del equipo/club, deporte, categoría/edad, N° de integrantes, nombre de contacto, teléfono, email, veces por semana deseadas, días y horario preferido, comentarios. El formulario **no confirma un cupo ni asigna entrenador automáticamente** — solo recolecta la solicitud con el horario deseado; alguien del equipo CEB debe revisar disponibilidad real de entrenador y espacio antes de responder con la propuesta. Notificación por correo configurada igual que Convenios (agregar destinatario en el mismo panel de *Form submission notifications* de Netlify — el formulario aparecerá como "solicitud-equipo" en la lista una vez desplegado).

## Pendientes resueltos (23-07-2026)

- ~~Precio y horario de Funcional Kids~~ — **Resuelto:** martes y jueves 18:00, $39.900/mes.
- ~~Taller de fuerza para niños~~ — **Retirado del ecosistema público** por decisión de Edgar; ya no aparece en la landing ni en la base de conocimiento.
- ~~Pilates Reformer Sede Barroso, planes y precios~~ — **Resuelto:** 12 sesiones/mes $120.000, Adulto Mayor 8 sesiones/mes $64.000. Publicado en la landing como acordeón propio en Membresías.
- ~~Precio y horario de Fundamentos~~ — **Resuelto** vía `Documento_Maestro_Fundamentos.md`: 2x semana $50.000/mes, 3x semana $70.000/mes, horario lunes a viernes (ver [02_Membresias_y_Precios.md](02_Membresias_y_Precios.md)). Publicado en la landing como acordeón propio en Membresías y actualizado en la tarjeta de Experiencias.
- ~~Horarios de Entrenamiento asistido y Musculación~~ — **Resuelto:** lunes a viernes 06:00-22:00 continuado, sábado 09:00-13:00 (mismo horario general del Studio). Publicado en las tarjetas de Experiencias.

## Pendientes resueltos (06-08-2026)

- ~~Precio de sesión suelta de Indoor Cycling~~ — **Resuelto:** $10.000/sesión, agregado al acordeón "Arma tu plan: sesiones sueltas" en Membresías (no estaba publicado antes).
- ~~Precio de clase suelta de Box Aktiva-T~~ — **Resuelto:** $6.000/clase (Cross Training o GAP), agregado como card adicional dentro del acordeón de Box en Membresías (no estaba publicado antes).
- ~~Cupo máximo de Fundamentos~~ — **Corregido de 7 a 6 personas** por clase, en la tarjeta de Experiencias, el acordeón de Membresías y la nota de horarios. Confirmado por Edgar (06-08-2026): es la capacidad real del espacio, no un error de dato. También corregido en la fuente original `Documento_Maestro_Fundamentos.md` (repo `ceb-aktivat-repo/landing-page`).
- ~~Posicionamiento de Fundamentos~~ — **Resuelto:** se quitó la frase "el paso previo ideal antes de sumarte a musculación o Pilates" de la tarjeta de Experiencias. Ahora se describe solo con lo esencial de la filosofía propia del programa (técnica antes que intensidad, grupos reducidos, sin comparaciones), sin presentarlo como preparación para otra disciplina — según lo pidió Edgar explícitamente.
- ~~Flujo "tarjeta → precio → WhatsApp"~~ — **Resuelto:** las tarjetas de la sección "Las experiencias" (Entrenamiento asistido, Musculación, Pilates Reformer, Indoor Cycling, Fundamentos, Cross Training, GAP) ahora tienen un botón "Ver valor →" que lleva directo al acordeón de precios correspondiente en Membresías (ya abierto, sin que la persona tenga que buscarlo), desde donde puede hacer clic directo en "Reservar por WhatsApp". Se reutilizó el sistema de deep-linking a acordeones que ya existía (usado antes por los links "Ver planes" del Ecosistema). Clínica formativa de fútbol y Funcional Kids quedaron sin este botón: Clínica no tiene precio público (deriva a WhatsApp) y Funcional Kids ya muestra su precio directo en la tarjeta.

## Pendientes resueltos — IA de WhatsApp (06-08-2026)

- ~~Bot de WhatsApp (Meta Business Agent) daba información antigua/incorrecta~~ — **Causa confirmada por Edgar:** la IA estaba completando datos desde el historial de chats anteriores (conversaciones reales con precios/horarios viejos), no solo desde el PDF de base de conocimiento subido. **Solución:** activar la opción "Ignorar chats anteriores" en la configuración del Meta Business Agent, para que solo use la web, el catálogo y el PDF como fuente.
- ~~Deep-linking a los formularios de Convenios y Solicitud de equipo~~ — **Resuelto:** se agregaron anclas `#solicitud-convenio` y `#solicitud-equipo` en `index.html` que abren esos modales directo (antes solo se abrían con clic en un botón, sin URL propia). Permite que el bot de WhatsApp derive con un link directo en vez de explicar el proceso.
- ~~Reglas de derivación del bot de WhatsApp~~ — **Resuelto:** instrucciones agregadas al campo de configuración del Meta Business Agent (ver `contenido landing page/WhatsApp IA - Meta Business Agent/Instrucciones_de_Personalidad.md`): convenios → link `#solicitud-convenio`, solicitud de equipo → link `#solicitud-equipo`, información técnica o conversar con un entrenador → deriva al número institucional personal de Edgar (+56 9 8403 9920), y si no hay información confirmada sobre algo, nunca inventar — siempre derivar a un asesor.
- ~~Medios de pago~~ — **Resuelto:** transferencia bancaria, efectivo y tarjeta de crédito. No hay pago ni checkout online — se coordina con el asesor al inscribirse. Ver [03_Politicas_y_Reglas_de_Uso.md](03_Politicas_y_Reglas_de_Uso.md).
