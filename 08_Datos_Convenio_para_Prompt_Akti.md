# Datos de Convenio a Solicitar — Propuesta de Actualización para el Prompt de Akti

Creado el 17-07-2026, actualizado el 20-07-2026 tras confirmar el **convenio Club Leones de la Patagonia** como modelo maestro (ver [04_Convenios_Corporativos.md](04_Convenios_Corporativos.md)). Se usa junto con el [Sistema de Convenios CEB](../Convenios/Sistema%20de%20Convenios%20CEB/README_Instrucciones_Convenios_CEB.md) (Google Sheets + Apps Script que genera el PDF de convenio).

Para que el flujo quede completo de punta a punta, cuando alguien consulta por convenio corporativo/institucional en WhatsApp, Akti debería recolectar los datos que alimentan la hoja de convenios — así quien recibe el lead solo copia y pega en el Sheet y genera el PDF, sin tener que volver a preguntar nada.

## Texto propuesto para agregar al prompt (sección nueva)

Sugerido insertarlo después de la sección "ENTRENAMIENTO PERSONALIZADO" y antes de "SEÑAL DE COMPRA" del prompt actual (ver [06_Prompt_Akti_Asistente_Ventas.md](06_Prompt_Akti_Asistente_Ventas.md)):

```
# CONVENIOS CORPORATIVOS E INSTITUCIONALES
Si una empresa, club deportivo o institución consulta por convenio para sus socios/colaboradores, no des porcentajes de descuento ni cotices tú mismo — recolecta los datos y deriva para que el equipo prepare la propuesta formal. El descuento varía por unidad (Box, Studio, Cafetería, Clínica) y lo define Dirección caso a caso.

Pide, UNO POR MENSAJE (nunca todos juntos):
1. Nombre de la organización (empresa, club, institución)
2. Nombre y cargo de la persona de contacto
3. Email y teléfono de contacto
4. Tipo de organización (empresa / club deportivo / institución) y rubro si aplica
5. Número aproximado de socios o colaboradores interesados
6. Qué unidades les interesan (Box, Studio, Cafetería, Clínica, o todo el ecosistema) — si no saben, no insistas, eso lo define el equipo

En cuanto tengas al menos nombre de organización + nombre de contacto + un dato de contacto (email o teléfono), cierra así:
"Perfecto, con esto el equipo prepara la propuesta de convenio con las condiciones para [nombre organización]. Te contactan a la brevedad."
Luego agrega: ##LEAD##

No inventes porcentajes de descuento ni condiciones del convenio — eso lo define Dirección caso a caso.
```

## Ajuste también necesario en "CUÁNDO DERIVAR"

Agregar un punto a la lista existente de derivación:
```
- Una empresa, club deportivo o institución consulta por convenio corporativo para sus socios/colaboradores.
```

## Cómo se conecta con el Sistema de Convenios CEB

| Dato que pide Akti | Columna en la hoja "Convenios" |
|---|---|
| Nombre de la organización | Nombre organización |
| Tipo de organización | Tipo de organización |
| Nombre de contacto | Nombre contacto |
| Cargo de contacto | Cargo contacto |
| Teléfono | Teléfono contacto |
| Email | Email contacto |
| N° de socios/colaboradores interesados | N° de socios/colaboradores estimado |
| Unidades de interés (Box/Studio/Cafetería/Clínica) | Incluye Box / Incluye Studio / Incluye Cafetería / Incluye Clínica |

Los campos que Akti **no** debe definir (% descuento por unidad, RUT, dirección de la organización, vigencia inicial, Pase Aktiva-T) los completa el equipo/Dirección directamente en el Sheet al preparar la propuesta, según lo acordado con cada organización.

## Nota
Este es un texto **propuesto**, no aplicado automáticamente al bot en producción. Edgar debe revisarlo y pegarlo en la configuración real de Akti cuando esté conforme.
