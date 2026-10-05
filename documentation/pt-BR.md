<!-- ELUCENIA technical documentation · canadian-c-spine-rule · pt-BR · no clinical/professional/rights approval -->

# Canadian C-Spine Rule

[condições, fontes e permissões](https://elucenia.org/pt-br/ferramentas/canadian-c-spine-rule)

## Como usar

Use a ferramenta no portal ou abra index.html em um servidor HTTP local. Selecione o idioma, preencha os campos e calcule.

## Entradas e unidades

### Critério de exclusão: idade \< 16 anos, Glasgow \< 15, sinais vitais anormais, trauma há mais de 48 h, trauma penetrante, paralisia aguda, doença vertebral conhecida/cirurgia cervical prévia, retorno para reavaliação da mesma lesão ou gravidez

`excl`

### Alto risco: idade ≥ 65 anos

`idade65`

### Alto risco: mecanismo perigoso (queda de ≥ 0,9 m ou 5 degraus, carga axial na cabeça, colisão em alta velocidade, capotamento ou ejeção, veículo recreativo motorizado, colisão de bicicleta)

`mecanismo`

### Alto risco: parestesias nas extremidades

`parestesia`

### Baixo risco: colisão traseira simples (sem veículo lançado ao trânsito oposto, impacto por ônibus/caminhão grande, capotamento ou impacto em alta velocidade)

`colisao`

### Baixo risco: sentado na sala de emergência

`sentado`

### Baixo risco: deambulou em algum momento após o trauma

`deambulou`

### Baixo risco: dor cervical de início tardio

`tardia`

### Baixo risco: sem dor à palpação na linha média cervical

`semdor`

### Consegue rodar ativamente o pescoço 45° para a direita e para a esquerda?

`rot`

opcional

- `0` — Não
- `1` — Sim
- `na` — Ainda não testado

### Trauma contuso há ≤ 48 h; idade ≥ 16 anos, Glasgow 15, sinais vitais normais e inclusão pela dor cervical ou lesão acima das clavículas + ausência de deambulação + mecanismo perigoso confirmados?

`contexto`

- `0` — Não
- `1` — Sim

## Edição do método

Stiell 2001; Canadian C-Spine Rule

## Fórmula documentada

Sequência: exclusões → fatores de alto risco → existência de fator de baixo risco → rotação ativa já avaliada clinicamente.

## Limites e população

Não orienta realizar movimentos cervicais. Rotação não avaliada produz resultado incompleto. Critério ausente não equivale a ausência de lesão.

## Referências

- [Stiell et al. · Canadian C-Spine Rule · artigo e critérios completos de 2001](https://jamanetwork.com/journals/jama/fullarticle/194296)

- [Stiell IG et al. The Canadian C-Spine Rule for radiography in alert and stable trauma patients. JAMA, 2001.](https://doi.org/10.1001/jama.286.15.1841)

- [Stiell IG et al. The Canadian C-Spine Rule versus the NEXUS low-risk criteria in patients with trauma. N Engl J Med, 2003.](https://doi.org/10.1056/NEJMoa031375)

## Reproduzir os testes técnicos

Execute node test.cjs na pasta raiz deste repositório para repetir os casos sintéticos registrados. As entradas, expectativas e tolerâncias originais são preservadas. Testes técnicos não constituem validação clínica.

```sh
node test.cjs
```

tool.json contém fontes, edição e escopo de revisão. examples.json conserva as entradas e expectativas sintéticas; results.json registra os resultados obtidos.

[Ficha e referências](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referência](../examples.json) · [results.json](../results.json)

## Revisão e condições de uso

Revisão clínica independente não realizada.

Esta interface é uma tradução autoral, não uma edição oficial ou certificada. Revisão clínica independente, revisão linguística profissional e autorização de direitos de instrumentos não foram realizadas.

Resultado da fórmula ou classificação. Interpretação, conduta e aplicabilidade dependem da avaliação profissional e da fonte selecionada.

## Licença e atribuição

Apache-2.0 aplica-se somente ao código da ELUCENIA. Os instrumentos, publicações, traduções e dados mantêm os direitos dos respectivos titulares. Preserve LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
