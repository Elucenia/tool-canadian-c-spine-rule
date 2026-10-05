<!-- ELUCENIA technical documentation · canadian-c-spine-rule · fr · no clinical/professional/rights approval -->

# Règle canadienne du rachis cervical

[conditions, sources et autorisations](https://elucenia.org/fr/outils/canadian-c-spine-rule)

## Mode d’emploi

Utilisez l’outil sur le portail ou ouvrez index.html via un serveur HTTP local. Sélectionnez la langue, remplissez les champs et lancez le calcul.

## Données d’entrée et unités

### Critère d’exclusion : âge \< 16 ans, Glasgow \< 15, constantes vitales anormales, traumatisme datant de plus de 48 h, traumatisme pénétrant, paralysie aiguë, maladie vertébrale connue/chirurgie cervicale antérieure, réévaluation de la même lésion ou grossesse

`excl`

### Haut risque : âge ≥ 65 ans

`idade65`

### Haut risque : mécanisme dangereux (chute ≥ 0,9 m ou 5 marches, charge axiale sur la tête, collision à grande vitesse, tonneau ou éjection, véhicule de loisirs motorisé, collision à vélo)

`mecanismo`

### Haut risque : paresthésies des extrémités

`parestesia`

### Faible risque : collision arrière simple (sans véhicule projeté dans la circulation opposée, choc par bus/gros camion, tonneau ou choc à grande vitesse)

`colisao`

### Faible risque : assis aux urgences

`sentado`

### Faible risque : a marché à un moment après le traumatisme

`deambulou`

### Faible risque : douleur cervicale d’apparition retardée

`tardia`

### Faible risque : absence de douleur à la palpation de la ligne médiane cervicale

`semdor`

### Peut tourner activement le cou de 45° à droite et à gauche ?

`rot`

facultatif

- `0` — Non
- `1` — Oui
- `na` — Non encore testé

### Traumatisme fermé datant de ≤ 48 h ; âge ≥ 16 ans, Glasgow 15, constantes normales et inclusion par douleur cervicale ou lésion au-dessus des clavicules + absence de marche + mécanisme dangereux confirmés ?

`contexto`

- `0` — Non
- `1` — Oui

## Édition de la méthode

Stiell 2001; Canadian C-Spine Rule

## Formule documentée

Séquence : exclusions → facteurs de risque élevé → présence d’un facteur de faible risque → rotation active déjà évaluée cliniquement.

## Limites et population

Ne donne pas de consigne pour effectuer des mouvements cervicaux. Une rotation non évaluée produit un résultat incomplet. L’absence d’un critère ne signifie pas l’absence de lésion.

## Références

- [Stiell et al. · Canadian C-Spine Rule · article et critères complets de 2001](https://jamanetwork.com/journals/jama/fullarticle/194296)

- [Stiell IG et al. The Canadian C-Spine Rule for radiography in alert and stable trauma patients. JAMA, 2001.](https://doi.org/10.1001/jama.286.15.1841)

- [Stiell IG et al. The Canadian C-Spine Rule versus the NEXUS low-risk criteria in patients with trauma. N Engl J Med, 2003.](https://doi.org/10.1056/NEJMoa031375)

## Reproduire les tests techniques

Exécutez node test.cjs dans le répertoire racine de ce dépôt pour reproduire les cas synthétiques enregistrés. Les données d’entrée, les résultats attendus et les tolérances d’origine sont conservés. Les tests techniques ne constituent pas une validation clinique.

```sh
node test.cjs
```

tool.json contient les sources, l’édition et le périmètre de la revue. examples.json conserve les données d’entrée et les résultats attendus des cas synthétiques ; results.json consigne les résultats obtenus.

[Fiche et références](../tool.json) · [Code JavaScript](../calculator.js) · [Cas de référence](../examples.json) · [results.json](../results.json)

## Revue et conditions d’utilisation

Aucune révision clinique indépendante n’a été effectuée.

Cette interface est une traduction réalisée par nos soins, et non une édition officielle ou certifiée. La revue clinique indépendante, la révision linguistique professionnelle et l’autorisation des droits sur les instruments n’ont pas été réalisées.

Résultat de la formule ou de la classification. L’interprétation, la conduite et l’applicabilité dépendent de l’évaluation professionnelle et de la source sélectionnée.

## Licence et attribution

Apache-2.0 s’applique uniquement au code d’ELUCENIA. Les droits sur les instruments, publications, traductions et données restent ceux de leurs titulaires respectifs. Conservez LICENSE et NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
