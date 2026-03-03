# RA2 — Catàleg de cotxes (HTML + CSS)

Aquest exercici avalua el **RA2: Utilitza llenguatges de marques per a la transmissió i presentació d’informació a través del web**, analitzant l’estructura dels documents i identificant-ne els elements.

Has de desenvolupar un **petit lloc web format per dues pàgines HTML**, dedicades a un catàleg de cotxes, utilitzant únicament **HTML5 i CSS3**.

Les dades de contingut s’han d’extreure del fitxer **`cars.json`**, però **NO s’ha de fer cap lectura automàtica**:
les dades s’han de **copiar manualment** a l’HTML.

* A la pàgina **Classics** s’avaluarà **Flexbox amb `flex-wrap`**.
* A la pàgina **Vintage** s’avaluarà **posicionament absolut**.

---

## Fitxer de dades (només informatiu)

A la carpeta del projecte hi haurà un arxiu:

* `cars.json`

Aquest fitxer conté una llista d’objectes amb aquest format:

```json
{
  "id": 8,
  "name": "EV1",
  "manufacturer": "General Motors",
  "year": 1996,
  "cylinder": "Electric",
  "image": "gmev1.png"
}
```

Recorda: **no l’has d’usar per generar el contingut**. Simplement serveix per saber quines dades has de posar a les targetes.

---

## Pàgines a lliurar

Has de crear **dues pàgines HTML** (una per llista). En aquest exercici **no es demana cap index**.

* `classics.html` → llista “Cotxes clàssics” (Flexbox + `flex-wrap`)
* `vintage.html` → llista “Cotxes vintage” (posicionament absolut)

> En el fitxer `cars.json` trobaràs quins elements han d’anar a cada pàgina. En aquesta prova es valorarà sobretot **l’HTML i el CSS**, no la lògica de classificació.

---

## Estructura del projecte

```
web
├── classics.html
├── vintage.html
├── styles.css
└── imatges/
    ├── *.png
```

---

## Pàgina 1 — `classics.html` (Flexbox + flex-wrap)

Aquesta pàgina ha de mostrar la llista **Cotxes clàssics**.

### Requisits de maquetació (avaluació principal)

* Les targetes s’han de distribuir amb **Flexbox**.
* **És obligatori** usar `flex-wrap: wrap;`.
* Les targetes han de saltar de línia correctament quan no hi hagi espai.
* Ha d’haver-hi separació coherent entre targetes (amb `gap`, per exemple).
* La pàgina ha de ser llegible en diferents amplades de finestra (sense media queries obligatòries).

---

## Pàgina 2 — `vintage.html` (Posicionament absolut)

Aquesta pàgina ha de mostrar la llista **Cotxes vintage**.

### Requisits de maquetació (avaluació principal)

* La col·locació de les targetes s’ha de fer amb:

  * un contenidor que actuï de referència (`position: relative;`)
  * i targetes amb `position: absolute;`
* Has de col·locar les targetes en una graella “manual” (per files i columnes), **sense usar Flexbox ni Grid** per distribuir-les.
* No cal que sigui responsive: aquí s’avalua sobretot que entenguis **com funciona l’absolut** i la referència del contenidor.

---

## Contingut obligatori de cada targeta (a les dues pàgines)

Cada targeta ha de mostrar, com a mínim:

* Imatge (`image`)
* Nom del cotxe (`name`)
* Fabricant (`manufacturer`)
* Any (`year`)
* Motor / cilindres (`cylinder`)

---

## Criteris d’avaluació

* `classics.html`: ús correcte de **Flexbox** amb **`flex-wrap`**, distribució i espaiats. (5 punts)
* `vintage.html`: ús correcte de **`position: absolute`** amb contenidor **`position: relative`**, col·locació manual clara. (5 punts)

* HTML ben estructurat (ús correcte de seccions, títols, jerarquia i semàntica bàsica).
* CSS ordenat i coherent (selectors clars, estils consistents, sense duplicacions absurdes).
* Targetes completes amb tota la informació requerida.

---
