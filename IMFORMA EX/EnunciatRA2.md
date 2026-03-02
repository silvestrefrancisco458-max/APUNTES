# RA2 — Meravelles del món (HTML + CSS)

## Context

Aquest exercici avalua el **RA2: Utilitza llenguatges de marques per a la transmissió i presentació d’informació a través del web**, analitzant l’estructura dels documents i identificant-ne els elements.

Has de desenvolupar un **petit lloc web format per dues pàgines HTML**, dedicades a les **meravelles del món**, utilitzant únicament **HTML5 i CSS3**.

Les dades de contingut s’han d’extreure del fitxer **`meravelles.json`**, però **NO s’ha de fer cap lectura automàtica**:  
les dades s’han de **copiar manualment** a l’HTML.

---

## Objectiu general

Crear dues pàgines web coherents i professionals:

- una pàgina per a les **meravelles antigues**
- una pàgina per a les **meravelles modernes**

Cada pàgina ha d’utilitzar un **sistema de maquetació diferent** i adaptar-se correctament a dispositius mòbils.

---

## Estructura del projecte

```
web
├── antigues.html
├── modernes.html
├── styles.css
└── imatges/
    ├── antic-*.png
    └── modern-*.png
```

---

## Restriccions obligatòries

- ✅ HTML5 + CSS3
- ✅ CSS en un únic fitxer extern (`styles.css`)
- ✅ Disseny responsive (mòbil i escriptori)
- ❌ JavaScript
- ❌ frameworks CSS
- ❌ CSS inline
- ❌ lectura automàtica del JSON

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
  - enllaç a **Meravelles antigues**
  - enllaç a **Meravelles modernes**

El menú:
- es manté visible en fer scroll
- s’adapta a mòbil (flex en columna o wrap)

---

## Peu de pàgina (comú)

Les dues pàgines han de tenir **el mateix peu de pàgina**, amb:

- Text: **“Exàmen RA2 – Meravelles del món”**
- Nom de l’alumne/a
- Any actual

---

## Pàgina 1: `antigues.html` — Meravelles antigues

### Contingut
Mostrar **exactament 7 meravelles antigues**, segons el fitxer `meravelles.json`.

Per a cada meravella s’ha de mostrar:

- Nom de la meravella
- Ciutat o ubicació
- Cultura
- Any (o període)
- Imatge corresponent de la carpeta `imatges/`

### Maquetació
- **Obligatori: Flexbox**
- Presentació en **targetes (cards)**

### Responsive
- Mòbil: 1 columna
- Escriptori: diverses columnes segons amplada

---

## Pàgina 2: `modernes.html` — Meravelles modernes

### Contingut
Mostrar **exactament 7 meravelles modernes**, segons el fitxer `meravelles.json`.

Per a cada meravella s’ha de mostrar:

- Nom de la meravella
- País o ubicació
- Any de construcció o reconeixement
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
- Colors neutres
- Almenys una pseudo-classe `:hover`

---

## Avaluació (10 punts)

La nota final d’aquest RA és de **0 a 10 punts**, obtinguda de la suma dels criteris següents:

### Estructura i bones pràctiques (2 punts)
- **1 punt**: HTML5 correcte i semàntic a les dues pàgines (`header`, `nav`, `main`, `section`, `footer`)
- **1 punt**: CSS extern únic, codi net i ben organitzat

### Navegació i elements comuns (2 punts)
- **1 punt**: Menú superior comú, funcional i amb `position: sticky`
- **1 punt**: Peu de pàgina comú amb text, nom i any correctes

### Pàgina de meravelles antigues (3 punts)
- **1 punt**: Es mostren les 7 meravelles antigues amb les dades correctes
- **1 punt**: Maquetació amb Flexbox ben aplicada
- **1 punt**: Adaptació correcta a mòbil (1 columna)

### Pàgina de meravelles modernes (3 punts)
- **1 punt**: Es mostren les 7 meravelles modernes amb les dades correctes
- **1 punt**: Maquetació amb CSS Grid ben aplicada
- **1 punt**: Adaptació correcta a mòbil i escriptori (canvi de columnes)

---

## Nota important

- No s’ha de llegir el JSON automàticament.
- Les dades copiades han de coincidir amb `meravelles.json`.
- L’incompliment de les restriccions pot comportar penalització o invalidació de l’exercici.
