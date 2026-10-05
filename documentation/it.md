<!-- ELUCENIA technical documentation · canadian-c-spine-rule · it · no clinical/professional/rights approval -->

# Canadian C-Spine Rule

[condizioni, fonti e autorizzazioni](https://elucenia.org/it/strumenti/canadian-c-spine-rule)

## Come usare

Usi lo strumento nel portale oppure apra index.html tramite un server HTTP locale. Selezioni la lingua, compili i campi ed esegua il calcolo.

## Dati di ingresso e unità

### Criterio di esclusione: età \< 16 anni, Glasgow \< 15, parametri vitali anomali, trauma da più di 48 h, trauma penetrante, paralisi acuta, malattia vertebrale nota/pregressa chirurgia cervicale, rivalutazione della stessa lesione o gravidanza

`excl`

### Alto rischio: età ≥ 65 anni

`idade65`

### Alto rischio: meccanismo pericoloso (caduta ≥ 0,9 m o 5 gradini, carico assiale sulla testa, collisione ad alta velocità, ribaltamento o eiezione, veicolo ricreativo motorizzato, collisione in bicicletta)

`mecanismo`

### Alto rischio: parestesie alle estremità

`parestesia`

### Basso rischio: semplice tamponamento (senza veicolo spinto nel traffico opposto, impatto con autobus/grande camion, ribaltamento o impatto ad alta velocità)

`colisao`

### Basso rischio: seduto in pronto soccorso

`sentado`

### Basso rischio: ha camminato in qualsiasi momento dopo il trauma

`deambulou`

### Basso rischio: insorgenza tardiva del dolore cervicale

`tardia`

### Basso rischio: assenza di dolorabilità sulla linea mediana cervicale

`semdor`

### Può ruotare attivamente il collo di 45° a destra e a sinistra?

`rot`

facoltativo

- `0` — No
- `1` — Sì
- `na` — Non ancora valutato

### Trauma contusivo da ≤ 48 h; età ≥ 16 anni, Glasgow 15, parametri vitali normali e inclusione per dolore cervicale o lesione sopra le clavicole + assenza di deambulazione + meccanismo pericoloso confermati?

`contexto`

- `0` — No
- `1` — Sì

## Edizione del metodo

Stiell 2001; Canadian C-Spine Rule

## Formula documentata

Sequenza: esclusioni → fattori di alto rischio → presenza di un fattore di basso rischio → rotazione attiva già valutata clinicamente.

## Limiti e popolazione

Non indica di eseguire movimenti cervicali. Una rotazione non valutata produce un risultato incompleto. L’assenza di un criterio non equivale ad assenza di lesione.

## Riferimenti

- [Stiell et al. · Canadian C-Spine Rule · articolo e criteri completi del 2001](https://jamanetwork.com/journals/jama/fullarticle/194296)

- [Stiell IG et al. The Canadian C-Spine Rule for radiography in alert and stable trauma patients. JAMA, 2001.](https://doi.org/10.1001/jama.286.15.1841)

- [Stiell IG et al. The Canadian C-Spine Rule versus the NEXUS low-risk criteria in patients with trauma. N Engl J Med, 2003.](https://doi.org/10.1056/NEJMoa031375)

## Riprodurre i test tecnici

Esegua node test.cjs nella cartella principale di questo repository per ripetere i casi sintetici registrati. Gli input, i risultati attesi e le tolleranze originali sono conservati. I test tecnici non costituiscono validazione clinica.

```sh
node test.cjs
```

tool.json contiene le fonti, l’edizione e l’ambito della revisione. examples.json conserva gli input e i risultati attesi dei casi sintetici; results.json registra i risultati ottenuti.

[Scheda e riferimenti](../tool.json) · [Codice JavaScript](../calculator.js) · [Casi di riferimento](../examples.json) · [results.json](../results.json)

## Revisione e condizioni d’uso

Non è stata effettuata una revisione clinica indipendente.

Questa interfaccia è una traduzione realizzata dagli autori, non un’edizione ufficiale o certificata. Non sono state eseguite la revisione clinica indipendente, la revisione linguistica professionale né la verifica delle autorizzazioni relative ai diritti sugli strumenti.

Risultato della formula o classificazione. Interpretazione, condotta e applicabilità dipendono dalla valutazione professionale e dalla fonte selezionata.

## Licenza e attribuzione

Apache-2.0 si applica solo al codice di ELUCENIA. I diritti su strumenti, pubblicazioni, traduzioni e dati restano ai rispettivi titolari. Conservi LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
