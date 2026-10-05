<!-- ELUCENIA technical documentation · canadian-c-spine-rule · en · no clinical/professional/rights approval -->

# Canadian C-Spine Rule

[conditions, sources and permissions](https://elucenia.org/en/tools/canadian-c-spine-rule)

## How to use

Use the tool in the portal or open index.html through a local HTTP server. Select the language, complete the fields and calculate.

## Inputs and units

### Exclusion criterion: age \< 16 years, Glasgow \< 15, abnormal vital signs, trauma more than 48 h ago, penetrating trauma, acute paralysis, known vertebral disease/prior cervical surgery, reassessment of the same injury or pregnancy

`excl`

### High risk: age ≥ 65 years

`idade65`

### High risk: dangerous mechanism (fall ≥ 0.9 m or 5 steps, axial load to the head, high-speed collision, rollover or ejection, motorized recreational vehicle, bicycle collision)

`mecanismo`

### High risk: paresthesias in the extremities

`parestesia`

### Low risk: simple rear-end collision (no vehicle pushed into oncoming traffic, impact by a bus/large truck, rollover or high-speed impact)

`colisao`

### Low risk: sitting in the emergency department

`sentado`

### Low risk: walked at any time after the trauma

`deambulou`

### Low risk: delayed onset of neck pain

`tardia`

### Low risk: no midline cervical tenderness

`semdor`

### Can actively rotate the neck 45° to the right and left?

`rot`

optional

- `0` — No
- `1` — Yes
- `na` — Not yet tested

### Blunt trauma ≤ 48 h ago; age ≥ 16 years, Glasgow 15, normal vital signs and inclusion by neck pain or injury above the clavicles + inability to walk + dangerous mechanism confirmed?

`contexto`

- `0` — No
- `1` — Yes

## Method edition

Stiell 2001; Canadian C-Spine Rule

## Documented formula

Sequence: exclusions → high-risk factors → presence of a low-risk factor → active rotation already clinically assessed.

## Limits and population

Does not instruct cervical movements. Unassessed rotation produces an incomplete result. An absent criterion does not mean an injury is absent.

## References

- [Stiell et al. · Canadian C-Spine Rule · complete 2001 article and criteria](https://jamanetwork.com/journals/jama/fullarticle/194296)

- [Stiell IG et al. The Canadian C-Spine Rule for radiography in alert and stable trauma patients. JAMA, 2001.](https://doi.org/10.1001/jama.286.15.1841)

- [Stiell IG et al. The Canadian C-Spine Rule versus the NEXUS low-risk criteria in patients with trauma. N Engl J Med, 2003.](https://doi.org/10.1056/NEJMoa031375)

## Reproduce the technical tests

Run node test.cjs in the root directory of this repository to repeat the recorded synthetic cases. Original inputs, expectations and tolerances are preserved. Technical tests do not constitute clinical validation.

```sh
node test.cjs
```

tool.json contains sources, edition and review scope. examples.json retains synthetic inputs and expectations; results.json records the obtained results.

[Record and references](../tool.json) · [JavaScript code](../calculator.js) · [Reference cases](../examples.json) · [results.json](../results.json)

## Review and conditions of use

Independent clinical review has not been performed.

This interface is an authorial translation, not an official or certified edition. Independent clinical review, professional language review and instrument rights clearance have not been performed.

Formula or classification result. Interpretation, care and applicability depend on professional assessment and the selected source.

## License and attribution

Apache-2.0 applies only to ELUCENIA code. Rights to instruments, publications, translations and data remain with their respective holders. Preserve LICENSE and NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
