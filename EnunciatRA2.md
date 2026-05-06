# RA2 — Déus víkings (HTML + CSS)

## Context

Aquest exercici avalua el **RA2: Utilitza llenguatges de marques per a la transmissió i presentació d'informació a través del web**, analitzant l'estructura dels documents i identificant-ne els elements.

Has de desenvolupar un **petit lloc web format per dues pàgines HTML**, dedicades als **déus víkings**, utilitzant únicament **HTML5 i CSS3**.

Les dades de contingut s'han d'extreure del fitxer **`deus.json`**, però **NO** s'ha de fer cap lectura automàtica:  
les dades s'han de **copiar manualment** a l'HTML.

---

## Objectiu general

Crear dues pàgines web coherents i professionals:

- una pàgina per als **déus d'Asgard**
- una pàgina per als **déus Vanir**

Cada pàgina ha d'utilitzar un **sistema de maquetació diferent** i adaptar-se correctament a dispositius mòbils.

---

## Estructura del projecte

```text
RA123-2026D/RA2/
├── deus.json
└── web
    ├── asgard.html
    ├── vanir.html
    ├── styles.css
    └── imatges/
        ├── asgard-*.
        └── vanir-*.
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

- `deus.json`

Aquest fitxer conté una llista d'objectes amb aquest format:

```json
{
  "id": 1,
  "nom": "Odin",
  "grup": "asgard",
  "residencia": "Valaskjalf",
  "domini": "Saviesa i guerra",
  "arxiu": "asgard-odin.svg"
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
  - enllaç a **Déus d'Asgard**
  - enllaç a **Déus Vanir**

El menú:

- es manté visible en fer scroll
- s'adapta a mòbil

---

## Peu de pàgina (comú)

Les dues pàgines han de tenir **el mateix peu de pàgina**, amb:

- Text: **"Examen RA2 - Déus víkings"**
- Nom de l'alumne/a
- Any actual

---

## Pàgina 1: `asgard.html` — Déus d'Asgard

### Contingut

Mostrar **exactament 7 déus d'Asgard**, segons el fitxer `deus.json`.

Per a cada déu s'ha de mostrar:

- Nom
- Residència o sala principal
- Domini o poder principal
- Imatge corresponent de la carpeta `imatges/`

### Maquetació

- **Obligatori: Flexbox**
- **És obligatori** usar `flex-wrap: wrap;`
- Presentació en **targetes**

### Responsive

- Mòbil: 1 columna
- Escriptori: diverses columnes segons amplada

---

## Pàgina 2: `vanir.html` — Déus Vanir

### Contingut

Mostrar **exactament 7 déus Vanir**, segons el fitxer `deus.json`.

Per a cada déu s'ha de mostrar:

- Nom
- Residència o regne associat
- Domini o poder principal
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
- Colors coherents amb la temàtica nòrdica
- Almenys una pseudo-classe `:hover`

---

## Avaluació (10 punts)

La nota final d'aquest RA és de **0 a 10 punts**, obtinguda de la suma dels criteris següents:

### Estructura i bones pràctiques (2 punts)

- **1 punt**: HTML5 correcte i semàntic a les dues pàgines (`header`, `nav`, `main`, `section`, `footer`)
- **1 punt**: CSS extern únic, codi net i ben organitzat

### Navegació i elements comuns (2 punts)

- **1 punt**: Menú superior comú, funcional i amb `position: sticky`
- **1 punt**: Peu de pàgina comú amb text, nom i any correctes

### Pàgina de déus d'Asgard (3 punts)

- **1 punt**: Es mostren els 7 déus d'Asgard amb les dades correctes
- **1 punt**: Maquetació amb Flexbox i `flex-wrap` ben aplicada
- **1 punt**: Adaptació correcta a mòbil

### Pàgina de déus Vanir (3 punts)

- **1 punt**: Es mostren els 7 déus Vanir amb les dades correctes
- **1 punt**: Maquetació amb CSS Grid ben aplicada
- **1 punt**: Adaptació correcta a mòbil i escriptori

---

## Nota important

- No s'ha de llegir el JSON automàticament.
- Les dades copiades han de coincidir amb `deus.json`.
- L'incompliment de les restriccions pot comportar penalització o invalidació de l'exercici.
