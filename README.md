# Webprogramozás kurzus értékelő kérdőív

Ez a repository a Webprogramozás kurzus záró beadandó feladatának megoldását tartalmazza.
A feladat egy reszponzív, struktúrált, dizájnos hallgatói visszajelző kérdőív
elkészítése volt, drótvázakkal együtt.

## A feladat

Reszponzív kérdőív tervezése és elkészítése a Webprogramozás kurzushoz az alábbi
követelményekkel:

- Drótváz (wireframe) készítése **monitorra és telefonra**
- **15 kérdés** a hallgatók elégedettségéről és fejlesztési javaslatairól
- Reszponzív, struktúrált, dizájnos megjelenés
- Csatolás az önéletrajz weboldalához (Kérdőív menüpont)

## Fájlszerkezet

```
.
├── kerdoiv.html             -- A kérdőív főoldala (új)
├── kerdoiv.css              -- A kérdőív stíluslapja (új)
├── wireframe_desktop.png    -- Drótváz asztali nézethez (1000px)
├── wireframe_mobile.png     -- Drótváz mobil nézethez (380px)
│
├── fooldal.html             -- Önéletrajz főoldal (frissítve: Kérdőív menüpont)
├── kedvenc_versem.html      -- Vers oldal (frissítve: Kérdőív menüpont)
├── hobbi.html               -- Iskola és hobbi oldal (frissítve: Kérdőív menüpont)
├── style.css                -- Önéletrajz stíluslapja
├── favicon.svg              -- Saját készítésű favicon
└── README.md                -- Ez a leírás
```

## A kérdőív szerkezete

A 15 kérdés három logikai csoportra van osztva, `<fieldset>` elemekkel:

### A) Általános elégedettség (1-5. kérdés)
- Általános elégedettség (5-skálás csillag-értékelés)
- Tananyag minősége
- Oktató felkészültsége
- Kurzus tempója
- Rangsorolás az eddigi tárgyak között

### B) Tartalmi visszajelzés (6-10. kérdés)
- Hasznos témakörök (több is választható)
- Bootstrap segítsége
- Tananyag mélysége
- Moodle segédanyagok hasznossága
- Vizsgakövetelmények világossága

### C) Fejlesztési javaslatok (11-15. kérdés)
- Mire szánjon több időt a kurzus (több is választható)
- Új témakör javaslat (szöveges)
- Részletes fejlesztési javaslatok (textarea)
- Ajánlanád-e másnak
- Egyéb megjegyzés (textarea)

## Használt technológiák és HTML elemek

A kérdőív az `Űrlapok` prezentációban tárgyalt összes elemet használja:

- `<form>` - method, action, autocomplete attribútumokkal
- `<fieldset>` és `<legend>` - csoportosítás
- `<label>` - minden mező felirattal
- `<input>` - radio, checkbox, text típusokkal
- `<select>` és `<option>` - lenyíló lista
- `<textarea>` - többsoros szövegmező
- `<button>` - submit és reset típusú gombok

## Reszponzív megjelenés

A weboldal három töréspontot használ a `Reszponzív weboldalak`
prezentáció ajánlása szerint:

| Töréspont | Leírás |
|-----------|--------|
| `> 768px` | Asztali nézet - vízszintes elrendezés |
| `≤ 768px` | Tablet nézet - rádió/checkbox elemek egymás alatt |
| `≤ 480px` | Mobil nézet - függőleges menü, teljes szélességű gombok |

## Megjelenítés

A weboldal megnyitásához egyszerűen kattints duplán a `kerdoiv.html` fájlra,
vagy nyisd meg egy webböngészőben. A navigációs menü segítségével szabadon
átnavigálhatsz az önéletrajz többi oldalára is.

## Validáció

A fájlok a W3C HTML5 és CSS validátoron hibátlanok:
- HTML5: https://validator.w3.org/
- CSS: https://jigsaw.w3.org/css-validator/

## Készítette

Baji Gabor &mdash; Milton Friedmann Egyetem, Webprogramozás kurzus, 2026 tavaszi félév

Neptun kód: DISEXN

## Megjegyzés

Ez a kérdőív bemutató jellegű (a feladat HTML és CSS készítésére fókuszál),
így a beküldés gomb csak demonstrációs célokat szolgál &mdash; valós szerver
oldali feldolgozás nincs mögötte.
