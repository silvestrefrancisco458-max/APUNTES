# RA3 — Pàgina interactiva “Animals del zoo” (HTML + CSS, sense JavaScript)

## Context

Aquest exercici avalua el **RA3: Accedeix i manipula documents web utilitzant llenguatges de guions de client**.

La manipulació del document web s’ha de realitzar **sense JavaScript**, utilitzant exclusivament **HTML i CSS**, mitjançant:
- inputs de tipus `checkbox` **ocults**
- etiquetes `<label>`
- pseudo-classes (`:checked`)
- transicions i/o animacions CSS
- posicionament (`absolute`, `z-index`)

---

## Objectiu

Crear una **pàgina interactiva** amb una escena de zoo utilitzant la imatge de fons `web/assets/background.png`.

La pàgina ha de mostrar **4 toggle buttons**, un per a cada animal, que permetin **mostrar i amagar** els animals sobre la imatge de fons:
- dofí
- jirafa
- hipopòtam
- cavall

Cada animal ha d’aparèixer i desaparèixer amb una **animació CSS** en la seva zona corresponent del mapa.

Tot el comportament interactiu s’ha de fer **només amb HTML i CSS**.

---

## Restriccions obligatòries

- ✅ HTML5 + CSS3
- ✅ CSS en fitxer extern (`styles.css`)
- ✅ toggle buttons controlats amb `checkbox` **ocults** + `label`
- ❌ JavaScript
- ❌ frameworks CSS
- ❌ CSS inline

Qualsevol ús de JavaScript **invalida l’exercici**.

---

## Recursos disponibles

Es proporcionaran les imatges següents dins de `web/assets/`:
- `background.png`
- `dolphin.png`
- `giraffe.png`
- `hippopotamus.png`
- `horse.png`

---

## Requisits visuals generals

### Fons de la pàgina
- El fons ha de ser **la imatge `background.png`**
- Ha d’ocupar **tot l’espai visible de la finestra**
- Els animals s’han de veure **superposats** al fons
- No cal adaptació a mòbil (no responsive)

### Zona de controls
- A la part superior de la pàgina hi ha d’haver **4 toggle buttons**
- Cada toggle ha d’estar clarament identificat amb el nom de l’animal
- Els toggles han de permetre activar o desactivar cada animal **de manera independent**
- Tot el sistema de controls s’ha de fer **només amb CSS i `checkbox` ocults**

---

## Control d’estat amb toggle buttons (obligatori)

Cada toggle ha d’estar implementat amb:
- un `input type="checkbox"` **ocult**
- un `<label>` associat que actuï com a botó

En fer clic al toggle:
- l’animal corresponent ha d’**aparèixer** o **desaparèixer**
- el control s’ha de fer amb `:checked`

⚠️ **L’estat de cada animal ha de ser independent de la resta.**
⚠️ **No es pot utilitzar JavaScript per afegir o treure classes, controlar events o canviar la visibilitat.**

---

## Animals i ubicació obligatòria

Els 4 animals han d’estar col·locats sobre la imatge de fons a les zones següents:

### Cavall
- Ha d’aparèixer a la **zona de l’estable**
- És a dir, a la part **inferior dreta** del fons, dins o davant del recinte de la granja

### Hipopòtam
- Ha d’aparèixer a l’**estany situat a l’esquerra de l’estable**
- És a dir, a la zona d’aigua de la part **inferior esquerra**

### Jirafa
- Ha d’aparèixer a la **zona amb l’arbre gran**
- És a dir, a la part **superior esquerra** del paisatge

### Dofí
- Ha d’aparèixer al **llac de la cascada**
- És a dir, a la zona d’aigua de la part **dreta**, sota la cascada

⚠️ No n’hi ha prou amb mostrar els animals: han d’estar **posicionats correctament i de manera coherent** respecte al paisatge.

---

## Animació d’aparició i desaparició (obligatori)

Quan un animal es mostri o s’amagui, ha de tenir una **animació visible**.

### Requisit mínim

L’efecte ha d’animar **com a mínim 3 propietats CSS**.

Per exemple, es poden combinar propietats com:
- `opacity`
- `transform`
- `filter`

També es poden utilitzar altres propietats animables si l’efecte és clar i coherent.

### Qualitat de l’animació

- L’entrada ha de ser **visible i progressiva**
- La sortida també ha de ser **suau i clara**
- L’efecte no pot ser un canvi instantani sense transició

---

## Implementació dels animals

- Cada animal ha de ser un element independent (per exemple `img` o `div` amb imatge)
- S’ha de posicionar amb:
  - `position: absolute` (o equivalent dins d’un contenidor relatiu)
  - `z-index` adequat per veure’l correctament sobre el fons
- La mida dels animals ha de ser coherent amb l’escena

---

## Organització del codi

- HTML estructurat i llegible
- CSS ordenat per blocs (fons, controls, animals, animacions)
- Ús coherent de classes
- Inputs ocults correctament (sense perdre funcionalitat)

---

## Avaluació (10 punts)

La nota final és de **0 a 10 punts**, obtinguda de la suma dels criteris següents:

### Toggle buttons i control d’estat (3 punts)
- **1 punt**: 4 toggle buttons funcionals
- **1 punt**: control correcte amb `checkbox`, `label` i `:checked`

### Ubicació dels animals (3 punts)
- **1 punt**: cada animal situat a la zona correcta del paisatge
- **1 punt**: mides i posicions coherents amb l’escena

### Animació d’aparició/desaparició (3 punts)
- **1 punt**: cada animal apareix i desapareix amb animació
- **1 punt**: l’animació utilitza almenys 3 propietats CSS

### Estructura i bones pràctiques (1 punts)
- **1 punt**: HTML i CSS nets, ordenats i ben formats
- **1 punt**: ús correcte de classes, posicionament i organització visual

---

## Entrega

web
- `index.html`
- `styles.css`
- carpeta `assets/` amb:
  - `background.png`
  - `dolphin.png`
  - `giraffe.png`
  - `hippopotamus.png`
  - `horse.png`
