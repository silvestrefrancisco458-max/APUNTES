# RA3 — Pàgina interactiva “Circuit de cotxes” (HTML + CSS, sense JavaScript)

## Context

Aquest exercici avalua el **RA3: Accedeix i manipula documents web utilitzant llenguatges de guions de client**.

La manipulació del document web s’ha de realitzar **sense JavaScript**, utilitzant exclusivament **HTML i CSS**, mitjançant:

* inputs de tipus `checkbox`
* etiquetes `<label>`
* pseudo-classes (`:checked`)
* animacions CSS (`transform`, `transition`, `animation`)
* posicionament (`position`, `z-index`)

---

## Objectiu

Crear una **pàgina interactiva** amb la temàtica **“Circuit de cotxes”** on:

* la pàgina mostra el **circuit com a fons** (imatge `circuit.png`)
* un **cotxe se superposa** al circuit i es mou amb una **animació en forma de triangle**
* l’animació es pot **activar/desactivar** amb un **botó toggle** a la part superior
* a cada tram del recorregut, el cotxe ha d’estar amb **l’angle correcte** (orientació coherent amb el moviment)

Tot el comportament interactiu s’ha de fer **únicament amb HTML i CSS**.

---

## Restriccions obligatòries

* ✅ HTML5 + CSS3
* ✅ CSS en fitxer extern (`styles.css`)
* ❌ JavaScript
* ❌ frameworks CSS
* ❌ CSS inline
* ❌ lectura automàtica de dades (JSON)

Qualsevol ús de JavaScript **invalida l’exercici**.

---

## Recursos disponibles

Es proporcionaran:

* `assets/circuit.png` (imatge de fons del circuit)
* `assets/cotxe.png` (imatge del cotxe amb vista superior)

---

## Requisits visuals generals

### Fons de la pàgina

* El fons ha de ser **la imatge `circuit.png`**
* Ha d’ocupar **tot l’espai visible de la finestra**
* El cotxe s’ha de veure **a sobre** del circuit (superposat)
* No cal adaptació a mòbil (no responsive)

---

## Control de l’animació amb toggle (obligatori)

A la **part superior** de la pàgina hi ha d’haver un **botó toggle** que controli l’animació.

### Control d’estat

* El toggle ha d’estar implementat amb:

  * un `input type="checkbox"` (pot estar ocult o estilitzat)
  * un `<label>` associat que actuï com a botó
* En activar/desactivar el toggle:

  * l’animació del cotxe **s’inicia** o **s’atura**
  * el control s’ha de fer amb `:checked` (sense JS)

---

## Cotxe (obligatori)

* El cotxe ha de ser un element (per exemple una `div` o `img`) posicionat amb:

  * `position: absolute` (o equivalent)
  * `z-index` per estar per sobre del fons
* La imatge del cotxe (`cotxe.png`) ha de tenir **vista superior** i mida raonable.

---

## Recorregut de l’animació: triangle (obligatori)

El cotxe s’ha de moure seguint un recorregut **triangular**, com a la imatge de referència de l’enunciat.

### Requisits del moviment

* El recorregut ha de tenir **3 trams rectes** (3 costats del triangle)
* Els **vèrtexs** han de ser **angulars** (sense corbes)
* El moviment ha de ser **cíclic** (quan acaba, torna a començar)

### Angle correcte del cotxe

A cada tram, el cotxe ha d’estar **orientat** segons la direcció del moviment:

* tram 1: orientació coherent amb el primer costat
* tram 2: orientació coherent amb el segon costat
* tram 3: orientació coherent amb el tercer costat

⚠️ No n’hi ha prou amb moure’l: **també s’ha de rotar** (amb `transform: rotate(...)`) als punts clau del recorregut.

---

## Implementació de l’animació (CSS)

* El moviment s’ha de fer amb `@keyframes`
* S’han d’utilitzar percentatges per definir:

  * posició (x/y) del cotxe
  * rotació del cotxe
* L’animació ha de ser:

  * clara
  * fluida
  * visible

### Control amb :checked

* Quan el toggle estigui activat:

  * el cotxe **té animació**
* Quan el toggle estigui desactivat:

  * el cotxe **no es mou** (animació aturada o inactiva)

---

## Organització del codi

* HTML estructurat i llegible
* CSS ordenat per blocs (fons, UI, cotxe, animació)
* Ús coherent de classes
* Inputs ocults correctament (sense eliminar funcionalitat)

---

## Avaluació 

La nota final és de **0 a 10 punts**, obtinguda de la suma dels criteris següents:

- Fons i composició, `circuit.png` com a fons i cotxe correctament superposat (2 punts)
- Botó de toggle a la part superior, que canvia actiu/inactiu al fer click (2 punts)
- Animació triangular del cotxe sobre el circuit (2 punts)
- Orientació del cotxe segon la posició a l'animació (2 punts)
- Activar/Desactivar l'animació amb el botó de toggle (2 punts)

---

## Entrega

web

* `index.html`
* `styles.css`
* carpeta `assets/` amb:

  * `circuit.png`
  * `cotxe.png`

---

## Recorregut del cotxe

El recorregut del cotxe ha de ser el que marca la següent fletxa groga.

No confonguis l'arxiu "explicacio.png" amb "circuit.png"

<img src="explicacio.png" />