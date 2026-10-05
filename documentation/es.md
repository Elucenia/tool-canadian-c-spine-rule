<!-- ELUCENIA technical documentation · canadian-c-spine-rule · es · no clinical/professional/rights approval -->

# Regla canadiense de columna cervical

[condiciones, fuentes y permisos](https://elucenia.org/es/herramientas/canadian-c-spine-rule)

## Cómo usar

Utilice la herramienta en el portal o abra index.html mediante un servidor HTTP local. Seleccione el idioma, complete los campos y calcule.

## Entradas y unidades

### Criterio de exclusión: edad \< 16 años, Glasgow \< 15, constantes vitales anormales, traumatismo hace más de 48 h, traumatismo penetrante, parálisis aguda, enfermedad vertebral conocida/cirugía cervical previa, reevaluación de la misma lesión o embarazo

`excl`

### Alto riesgo: edad ≥ 65 años

`idade65`

### Alto riesgo: mecanismo peligroso (caída ≥ 0,9 m o 5 escalones, carga axial en la cabeza, colisión a alta velocidad, vuelco o eyección, vehículo recreativo motorizado, colisión de bicicleta)

`mecanismo`

### Alto riesgo: parestesias en las extremidades

`parestesia`

### Bajo riesgo: colisión trasera simple (sin vehículo desplazado al tráfico contrario, impacto por autobús/camión grande, vuelco o impacto a alta velocidad)

`colisao`

### Bajo riesgo: sentado en urgencias

`sentado`

### Bajo riesgo: caminó en algún momento después del traumatismo

`deambulou`

### Bajo riesgo: inicio tardío de dolor cervical

`tardia`

### Bajo riesgo: sin dolor a la palpación de la línea media cervical

`semdor`

### ¿Puede girar activamente el cuello 45° a la derecha y a la izquierda?

`rot`

opcional

- `0` — No
- `1` — Sí
- `na` — Aún no evaluado

### ¿Traumatismo cerrado hace ≤ 48 h; edad ≥ 16 años, Glasgow 15, constantes normales e inclusión por dolor cervical o lesión sobre las clavículas + ausencia de deambulación + mecanismo peligroso confirmados?

`contexto`

- `0` — No
- `1` — Sí

## Edición del método

Stiell 2001; Canadian C-Spine Rule

## Fórmula documentada

Secuencia: exclusiones → factores de alto riesgo → existencia de un factor de bajo riesgo → rotación activa ya evaluada clínicamente.

## Límites y población

No indica realizar movimientos cervicales. Una rotación no evaluada genera un resultado incompleto. La ausencia de un criterio no equivale a ausencia de lesión.

## Referencias

- [Stiell et al. · Canadian C-Spine Rule · artículo y criterios completos de 2001](https://jamanetwork.com/journals/jama/fullarticle/194296)

- [Stiell IG et al. The Canadian C-Spine Rule for radiography in alert and stable trauma patients. JAMA, 2001.](https://doi.org/10.1001/jama.286.15.1841)

- [Stiell IG et al. The Canadian C-Spine Rule versus the NEXUS low-risk criteria in patients with trauma. N Engl J Med, 2003.](https://doi.org/10.1056/NEJMoa031375)

## Reproducir las pruebas técnicas

Ejecute node test.cjs en el directorio raíz de este repositorio para repetir los casos sintéticos registrados. Se conservan las entradas, los resultados esperados y las tolerancias originales. Las pruebas técnicas no constituyen validación clínica.

```sh
node test.cjs
```

tool.json contiene las fuentes, la edición y el alcance de la revisión. examples.json conserva las entradas y los resultados esperados de los casos sintéticos; results.json registra los resultados obtenidos.

[Ficha y referencias](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referencia](../examples.json) · [results.json](../results.json)

## Revisión y condiciones de uso

No se ha realizado una revisión clínica independiente.

Esta interfaz es una traducción de elaboración propia, no una edición oficial o certificada. No se han realizado la revisión clínica independiente, la revisión lingüística profesional ni la autorización de derechos de los instrumentos.

Resultado de la fórmula o clasificación. La interpretación, la conducta y la aplicabilidad dependen de la evaluación profesional y de la fuente seleccionada.

## Licencia y atribución

Apache-2.0 se aplica únicamente al código de ELUCENIA. Los derechos de los instrumentos, publicaciones, traducciones y datos permanecen en manos de sus respectivos titulares. Conserve LICENSE y NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
