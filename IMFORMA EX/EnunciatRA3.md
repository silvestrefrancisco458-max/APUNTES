# RA3 — Pàgina interactiva “Animals de la Garrotxa” (HTML + CSS, sense JavaScript)

## Context

Aquest exercici avalua el **RA3: Accedeix i manipula documents web utilitzant llenguatges de guions de client**.

La manipulació del document web s’ha de realitzar **sense JavaScript**, utilitzant exclusivament **HTML i CSS**, mitjançant:
- inputs de tipus `checkbox`
- etiquetes `<label>`
- pseudo-classes (`:checked`)
- animacions CSS (`transform`, `transition`)

---

## Objectiu

Crear un **pàgina interactiva** amb la temàtica **“Animals de la Garrotxa”**, format per **targetes giratòries (flip cards)**.

Cada targeta representa un animal i pot girar de manera **independent** en fer-hi clic, mostrant informació diferent a la cara frontal i a la cara posterior.

Tot el comportament interactiu s’ha de fer **únicament amb HTML i CSS**.

---

## Restriccions obligatòries

- ✅ HTML5 + CSS3
- ✅ CSS en fitxer extern (`styles.css`)
- ❌ JavaScript
- ❌ frameworks CSS
- ❌ CSS inline
- ❌ lectura automàtica de dades (JSON)

Qualsevol ús de JavaScript **invalida l’exercici**.

---

## Recursos disponibles

Es proporcionaran:
- Imatge de **fons de la pàgina**
- Imatges dels animals
- Fitxer `animals.json` amb la informació dels animals

⚠️ **El fitxer `animals.json` NO s’ha d’importar ni llegir automàticament.**  
S’ha d’utilitzar **només com a font d’informació**, copiant manualment les dades a l’HTML.

---

## Requisits visuals generals

### Fons de la pàgina
- El fons ha de ser **una imatge**
- Ha d’ocupar **tot l’espai visible de la finestra**
- Ha de tenir un filtre CSS que li canvii el color per destacar les targetes
- No cal adaptació a mòbil (no responsive)

---

## Targetes d’animals (obligatori)

S’han de crear **3 targetes**, una per a cada animal a escollir del fitxer `animals.json`.

### Control d’estat
- Cada targeta ha de tenir:
  - un `input type="checkbox"` **ocult**
  - un `<label>` associat
- En fer clic sobre la targeta (label), el checkbox:
  - s’activa o es desactiva
  - controla l’animació de gir

⚠️ **L’estat de cada targeta ha de ser independent de les altres.**

---

## Cara frontal de la targeta

La **cara frontal** ha de mostrar:

- Imatge de l’animal
- Nom de l’animal a la part inferior
- El nom ha d’estar dins d’un element estilitzat (label o banda inferior)

---

## Cara posterior de la targeta

La **cara posterior** ha de mostrar la informació següent (segons `animals.json`):

- Tipus d’alimentació:
  - herbívor o carnívor
- Activitat:
  - diürn o nocturn
- Esperança de vida aproximada (anys)

---

## Animació de gir (flip)

- Les targetes han de tenir una **animació de gir en 3D**
- El gir ha d’estar controlat per:
  - l’estat `:checked` del checkbox
- L’animació ha de ser:
  - clara
  - fluida
  - visible

---

## Organització del codi

- HTML estructurat i llegible
- CSS ordenat per blocs
- Ús coherent de classes
- Inputs ocults correctament (sense eliminar funcionalitat)

---

## Avaluació (10 punts)

La nota final és de **0 a 10 punts**, obtinguda de la suma dels criteris següents:

### Control d’estat amb CSS (4 punts)
- **1 punt**: ús correcte de `checkbox` ocults
- **1 punt**: ús correcte de `<label>` per activar el gir
- **1 punt**: estat independent de cada targeta
- **1 punt**: control del gir mitjançant `:checked`

### Targetes i contingut (3 punts)
- **1 punt**: 3 targetes funcionals
- **1 punt**: cara frontal amb imatge i nom correctes
- **1 punt**: cara posterior amb la informació correcta segons `animals.json`

### Animació de gir (2 punts)
- **1 punt**: animació de flip CSS implementada
- **1 punt**: animació clara i fluida

### Estructura i bones pràctiques (1 punt)
- **1 punt**: HTML i CSS nets, ordenats i ben formats

---

## Entrega

web
- `index.html`
- `styles.css`
- carpeta `assets/` amb:
  - imatge de fons
  - imatges dels animals

---

## Nota final

Aquest exercici avalua la capacitat de:
- controlar l’estat d’elements web
- manipular el document amb CSS
- crear interactivitat **sense JavaScript**
