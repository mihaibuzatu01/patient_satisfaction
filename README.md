# Patient-Reported Measures Lab — V1

Aplicație educațională statică în limba română pentru clasificarea întrebărilor despre opinia pacientului, PREMs, PROMs și satisfacția globală și alegerea momentului de colectare.

## Publicare pe GitHub Pages
1. Creează un repository GitHub public, de exemplu `patient-measures-lab`.
2. Încarcă fișierele `index.html`, `questions.js`, `app.js` în rădăcina repository-ului (nu încărca numai arhiva ZIP).
3. Deschide **Settings → Pages → Build and deployment**, selectează **Deploy from a branch**, branch `main`, folder `/ (root)` și salvează.
4. După publicare, deschide URL-ul afișat de GitHub Pages.

## Conținut V1
- Mod A: etapă selectată înainte de clasificare.
- Mod B: identificarea etapei pornind de la item.
- Nivel 1: clasificare; nivel 2: clasificare și moment; nivel 3: include itemi defectuoși.
- Raport detaliat, tipărire/salvare ca PDF din browser și export CSV.
- Nu colectează și nu transmite răspunsuri către un server.

## Limitări și metodologie
- Banca inițială conține 24 de itemi demonstrativi originali. Nu sunt itemi ai unor instrumente psihometrice validate.
- La modul B, alegerea oricărei etape acceptate este corectă; V1 nu cere selecție multiplă.
- Nivelul 3 adaugă întrebări defectuoase, dar nu are încă exercițiu de rescriere liberă.
- Scorurile sunt formative, nu o certificare de competență.
- Banca trebuie revizuită de experți înainte de utilizarea într-un program formal de evaluare.

## Personalizare
Editează `questions.js`: fiecare item are `q` (text), `cat` (`op`, `prem`, `prom`, `sat`, `flawed`), `stages` (lista etapelor acceptate), `why` (explicație). Nu sunt necesare biblioteci externe.


## Configurație V1 actualizată
Fiecare sesiune conține exact 12 întrebări (3 opinie, 3 PREMs, 3 PROMs, 3 satisfacție globală), amestecate aleatoriu. Banca are cel puțin 12 itemi pentru fiecare categorie. În modul A, etapa aleasă este contextul de evaluare; pot apărea intenționat întrebări nepotrivite acelei etape pentru a testa selecția temporală. Itemii ambigui sunt păstrați în bancă pentru extinderi ulterioare, dar nu intră în scorul echilibrat V1.
