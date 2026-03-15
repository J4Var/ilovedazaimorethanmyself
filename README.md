# 🍸 The Golden Shaker | Casino Royale Menu

[![GitHub Pages](https://img.shields.io/badge/Live_Demo-Online-gold?style=for-the-badge&logo=github)]( https://j4var.github.io/ilovedazaimorethanmyself/)

> "A drink is not just a liquid; it's an entrance to a different world."

Vitajte v exkluzívnom nápojovom lístku inšpirovanom atmosférou luxusných kasín. Tento projekt je ukážkou dynamického spracovania dát z externého rozhrania v elegantnom vizuálnom šate.

---

## ♦️ O Projekte
Tento projekt vznikol ako zadanie na hodinu **Základov programovania**. Cieľom bolo vytvoriť dynamickú webovú stránku, ktorá nespolieha na statické HTML, ale čerpá informácie v reálnom čase.

### Hlavné funkcie:
* **Dynamický Fetch:** Dáta o koktailoch sú sťahované z `boozeapi.com`.
* **Casino Rich Design:** Luxusný vizuál so zlatými akcentmi, elegantnou typografiou a plynulými animáciami.
* **DOM Manipulácia:** Generovanie prvkov pomocou JavaScriptu (`appendChild`).

---

## ♣️ Použité technológie
* **HTML5** – Štruktúra menu.
* **CSS3** – Casino Royale vizuál (zlaté gradienty, hover efekty).
* **JavaScript (ES6)** – Srdce aplikácie (asynchrónne volanie `fetch`).
* **GitHub Pages** – Hosting projektu.

---

## ♥️ Ako to funguje? (Technické okienko)

Aplikácia po načítaní stránky spustí asynchrónnu funkciu, ktorá osloví API server. Prijaté dáta (vo formáte JSON) prejdú cyklom, ktorý pre každý drink vytvorí nový objekt typu `div.card`. Tento objekt je následne "prilepený" na stránku.

```javascript
// Ukážka kľúčovej logiky
fetch(url)
  .then(res => res.json())
  .then(data => container.appendChild(createCard(data)));
