# RA2 — Animals mitològics grecs (HTML + CSS)

## Context

Aquest exercici avalua el **RA2: Utilitza llenguatges de marques per a la transmissió i presentació d'informació a través del web**, analitzant l'estructura dels documents i identificant-ne els elements.

Has de desenvolupar un **petit lloc web format per dues pàgines HTML**, dedicades als **animals mitològics grecs**, utilitzant únicament **HTML5 i CSS3**.

Les dades de contingut s'han d'extreure del fitxer **`criatures.json`**, però **NO** s'ha de fer cap lectura automàtica:  
les dades s'han de **copiar manualment** a l'HTML.

---

## Objectiu general

Crear dues pàgines web coherents i professionals:

- una pàgina per a les **criatures terrestres**
- una pàgina per a les **criatures alades**

Cada pàgina ha d'utilitzar un **sistema de maquetació diferent** i adaptar-se correctament a dispositius mòbils.

---

## Estructura del projecte

```text
RA123-2026C/RA2/
├── criatures.json
└── web
    ├── terrestres.html
    ├── alades.html
    ├── styles.css
    └── imatges/
        ├── terrestre-*
        └── alada-*
```

---

## Restriccions obligatòries

- HTML5 + CSS3
- CSS en un únic fitxer extern (`styles.css`)
- Disseny responsive (mòbil i escriptori)
- No JavaScript
- No frameworks CSS
- No CSS inline
- No lectura automàtica del JSON

---

## Fitxer de dades

A la carpeta del projecte hi haurà un arxiu:

- `criatures.json`

Aquest fitxer conté una llista d'objectes amb aquest format:

```json
{
  "id": 1,
  "nom": "Minotaure",
  "grup": "terrestre",
  "origen": "Creta",
  "habilitat": "Força descomunal",
  "arxiu": "terrestre-minotaure.svg"
}
```

Recorda: **no l'has d'usar per generar el contingut**. Només serveix per saber quines dades has de posar a les targetes.

---

## Navegació comuna (obligatòria)

### Menú superior

- Visible a totes les pàgines
- Posicionament:

```css
position: sticky;
top: 0;
```

- Conté:
  - enllaç a **Criatures terrestres**
  - enllaç a **Criatures alades**

El menú:

- es manté visible en fer scroll
- s'adapta a mòbil

---

## Peu de pàgina (comú)

Les dues pàgines han de tenir **el mateix peu de pàgina**, amb:

- Text: **"Examen RA2 - Animals mitològics grecs"**
- Nom de l'alumne/a
- Any actual

---

## Pàgina 1: `terrestres.html` — Criatures terrestres

### Contingut

Mostrar **exactament 7 criatures terrestres**, segons el fitxer `criatures.json`.

Per a cada criatura s'ha de mostrar:

- Nom
- Origen o lloc mític
- Habilitat principal
- Imatge corresponent de la carpeta `imatges/`

### Maquetació

- **Obligatori: Flexbox**
- **És obligatori** usar `flex-wrap: wrap;`
- Presentació en **targetes**

### Responsive

- Mòbil: 1 columna
- Escriptori: diverses columnes segons amplada

---

## Pàgina 2: `alades.html` — Criatures alades

### Contingut

Mostrar **exactament 7 criatures alades**, segons el fitxer `criatures.json`.

Per a cada criatura s'ha de mostrar:

- Nom
- Origen o lloc mític
- Habilitat principal
- Imatge corresponent de la carpeta `imatges/`

### Maquetació

- **Obligatori: CSS Grid**

### Responsive

- Mòbil: 1 columna
- Tauleta: 2 columnes
- Escriptori: 3 o 4 columnes

---

## Estil i presentació (comú)

- Tipografia llegible
- Espaiat coherent
- Colors coherents amb la temàtica
- Almenys una pseudo-classe `:hover`

---

## Avaluació (10 punts)

La nota final d'aquest RA és de **0 a 10 punts**, obtinguda de la suma dels criteris següents:

### Estructura i bones pràctiques (2 punts)

- HTML5 correcte i semàntic a les dues pàgines (`header`, `nav`, `main`, `section`, `footer`)
- CSS extern únic, codi net i ben organitzat

### Navegació i elements comuns (2 punts)

- Menú superior comú, funcional i amb `position: sticky`
- Peu de pàgina comú amb text, nom i any correctes

### Pàgina de criatures terrestres (3 punts)

- Es mostren les 7 criatures terrestres amb les dades correctes
- Maquetació amb Flexbox i `flex-wrap` ben aplicada
- Adaptació correcta a mòbil

### Pàgina de criatures alades (3 punts)

- Es mostren les 7 criatures alades amb les dades correctes
- Maquetació amb CSS Grid ben aplicada
- Adaptació correcta a mòbil i escriptori

---

## Nota important

- No s'ha de llegir el JSON automàticament.
- Les dades copiades han de coincidir amb `criatures.json`.
- L'incompliment de les restriccions pot comportar penalització o invalidació de l'exercici.
