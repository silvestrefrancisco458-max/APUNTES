# RA3 — Pàgina interactiva "Curs de programació"

## Context

Aquest exercici avalua el **RA3: Accedeix i manipula documents web utilitzant llenguatges de guions de client**.

La manipulació del document web s’ha de realitzar **sense JavaScript**, utilitzant exclusivament **HTML i CSS**, mitjançant:
- inputs de tipus `checkbox`
- etiquetes `<label>`
- pseudo-classes (`:checked`)
- transicions CSS (`transition`)
- control de visibilitat i mida (`max-height`, `overflow`)

---

## Objectiu

Crear una **pàgina interactiva**, formada per una **llista collapsible**, amb blocs desplegables:

<center>
<video height="400" controls autoplay loop>
  <source src="./collapsible.mov" type="video/mp4">
  El teu navegador no suporta la reproducció de vídeo.
</video>
</center>

Cada bloc de la llista representa un apartat del curs i ha de poder-se **obrir i tancar de manera independent** en fer-hi clic.

L’efecte ha de seguir la idea d’un **collapsible tipus W3Schools**, però en aquest exercici s’ha d’implementar **sense JavaScript**, utilitzant únicament `checkbox` ocults i CSS.

Tot el comportament interactiu s’ha de fer **només amb HTML i CSS**.

---

## Restriccions obligatòries

- ✅ HTML5 + CSS3
- ✅ CSS en fitxer extern (`styles.css`)
- ✅ llista collapsible controlada amb `checkbox` + `label`
- ❌ JavaScript
- ❌ frameworks CSS
- ❌ CSS inline
- ❌ lectura automàtica de dades (JSON)

Qualsevol ús de JavaScript **invalida l’exercici**.

---

## Recursos disponibles

Es proporcionarà:
- `curs-html-css.json` amb els títols dels blocs i els continguts de cada apartat

⚠️ **El fitxer `curs-html-css.json` NO s’ha d’importar ni llegir automàticament.**  
S’ha d’utilitzar **només com a font d’informació**, copiant manualment els textos a l’HTML.

---

## Requisits visuals generals

### Aspecte de la pàgina
- La pàgina ha de tenir un **títol principal** relacionat amb el curs
- La llista collapsible ha d’estar **centrada o ben distribuïda**
- Cada apartat ha de semblar un **bloc interactiu clarament clicable**
- El disseny ha de ser net i coherent amb la temàtica formativa
- No cal adaptació a mòbil (no responsive)

---

## Llista collapsible del curs (obligatori)

S’han de crear **5 blocs collapsibles**, corresponents als apartats del fitxer `curs-html-css.json`.

### Control d’estat

Cada bloc ha de tenir:
- un `input type="checkbox"` **ocult**
- un `<label>` associat que actuï com a capçalera clicable
- un contenidor amb el contingut intern del bloc

En fer clic sobre el títol (`label`):
- el bloc s’ha d’**obrir o tancar**
- el control s’ha de fer amb `:checked`

⚠️ **L’estat de cada bloc ha de ser independent de la resta.**

---

## Contingut de cada bloc

La part visible de cada capçalera ha de mostrar:
- el **títol de l’apartat**

La zona desplegable de cada bloc ha de mostrar:
- la **descripció** de l’apartat
- una **llista d’ítems** (`<ul>` i `<li>`) amb els continguts del mòdul

Tots els textos han de coincidir amb la informació del fitxer `curs-html-css.json`.

---

## Comportament visual del collapsible

- El contingut ha d’estar **amagat per defecte**
- En activar el `checkbox`, el contingut s’ha de **mostrar**
- L’obertura i tancament han de tenir una **transició visual suau**
- Cal utilitzar propietats CSS adequades, per exemple:
  - `max-height`
  - `overflow`
  - `transition`

### Indicador visual

Cada capçalera ha de mostrar també un indicador visual d’estat:
- per exemple un símbol `+` / `−`
- o una fletxa que canviï en obrir/tancar

Aquest canvi també s’ha de controlar **només amb CSS**.

---

## Organització del codi

- HTML estructurat i llegible
- CSS ordenat per blocs
- Ús coherent de classes
- Inputs ocults correctament (sense perdre accessibilitat bàsica)
- Estructura semàntica correcta per a títols i llistes

---

## Avaluació (10 punts)

La nota final és de **0 a 10 punts**, obtinguda de la suma dels criteris següents:

### Control d’estat amb CSS (4 punts)
- **2 punts**: ús correcte de `checkbox` ocults i  `<label>` per obrir i tancar cada bloc
- **2 punts**: estat independent de cada apartat amb el control mitjançant `:checked`

### Llista i contingut (3 punts)
- 5 blocs collapsibles funcionals amb els títols i descripcions correctes segons `curs-html-css.json`
- llistes interiors correctament construïdes amb `<ul>` i `<li>`

### Presentació i transició visual (3 punts)
- obertura/tancament del contingut amb transició CSS amb l'indicador visual d’estat implementat correctament
- HTML i CSS nets, ordenats i ben formats

---

## Entrega

web
- `web/index.html`
- `web/styles.css`
