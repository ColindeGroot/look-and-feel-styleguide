# Styleguide

Ontwerp en maak met een team een styleguide om te gebruiken voor een opdracht van een opdrachtgever.
![Schermafbeelding 2024-11-15 094435](https://github.com/user-attachments/assets/f12f05be-b6c1-4c98-b75f-3290959d8f1c)

![Schermafbeelding 2024-11-15 094446](https://github.com/user-attachments/assets/23ed62cf-57bd-4381-a77f-2fb8c6fddeb6)

![Schermafbeelding 2024-11-15 094524](https://github.com/user-attachments/assets/4b44bb43-ca1e-4070-8820-ebddf074a3f5)

## README: Styleguide Documentatie

Deze README beschrijft de opzet van de styleguide en legt uit hoe de CSS-code in de stylesheet kan worden toegepast. De styleguide is gestructureerd rondom variabelen, typografie, knoppen en ankers, met een focus op consistentie, schaalbaarheid en toegankelijkheid.

---

### **Inhoud van de Styleguide**

#### **Globale CSS-instellingen**

De `body` bevat globale standaardinstellingen:

```css
body {
    padding: 0px;
    box-sizing: border-box;
}
```

1. **Padding** is ingesteld op `0px` om ongewenste marges te voorkomen.
2. **Box-sizing** is ingesteld op `border-box` zodat padding en borders worden meegenomen in de totale afmetingen van elementen.

---

#### **CSS-Variabelen**

CSS-variabelen worden gebruikt om consistentie te waarborgen en onderhoud te vereenvoudigen. Ze zijn gedefinieerd in de `body` en omvatten:

1. **Lettertypen (`font-family`)**:
   ```css
   --vag-rund: Arial, Helvetica, sans-serif;
   --open-sans: "Open Sans";
   ```

2. **Lettergroottes (`font-size`)**:
   ```css
   --font-size-xl: 2em; /* Extra groot */
   --font-size-l: 1.2em; /* Groot */
   --font-size-m: 1em; /* Normaal */
   --font-size-s: 0.875em; /* Klein */
   ```

3. **Lettergewichten (`font-weight`)**:
   ```css
   --light: 400; /* Licht */
   --normal: 500; /* Normaal */
   --bold: 600; /* Vet */
   ```

4. **Kleuren (`color`)**:
   ```css
   --darkred: #6A0025;
   --accentred: #d2b2bd;
   --white: #fff;
   --lightred: #F0E5E9;
   --black: #1F000B;
   ```

Gebruik van variabelen:
```css
color: var(--darkred);
font-size: var(--font-size-l);
```

---

#### **Typografie**

De styleguide definieert stijlen voor koppen (`h1`, `h2`, `h3`) en paragrafen (`p`):

- **Koppen**:
   - `h1`: Grote kop, gebruikt het lettertype `--vag-rund`, met een zwarte kleur en ruime marges.
   - `h2`: Iets kleinere kop met dezelfde stijl als `h1`.
   - `h3`: Nog kleiner en compacte marges.

   ```css
   h1 {
       font-family: var(--vag-rund);
       font-size: var(--font-size-xl);
       color: var(--black);
       margin: 50px 0px;
   }

   h2 {
       font-family: var(--vag-rund);
       font-size: var(--font-size-l);
   }

   h3 {
       font-size: var(--font-size-m);
       margin-top: 5px;
   }
   ```

- **Paragrafen**:
   - Gebruik van `--open-sans` voor leesbaarheid.
   ```css
   p {
       font-family: var(--open-sans);
       font-size: var(--font-size-s);
   }
   ```

---

#### **Knoppen en Links**

De styleguide biedt generieke stijlen voor knoppen en ankers, met extra klassen voor specifieke stijlen.

1. **Ankers (`a`)**:
   - Rode kleur die het merk weerspiegelt.
   ```css
   a {
       color: var(--darkred);
   }
   ```

2. **Knoppen (`button`)**:
   - Basisspanning en afgeronde hoeken.
   ```css
   button {
       padding: 16px 30px;
       color: var(--white);
       align-items: center;
       border-radius: 10px;
   }
   ```

3. **Specifieke knoppenstijlen**:
   - **Call-to-action knop** (`.cta-btn`):
     - Zwarte achtergrond, die bij hover lichtrood wordt.
     ```css
     .cta-btn {
         background-color: var(--black);
     }

     .cta-btn:hover {
         background-color: var(--lightred);
         color: var(--black);
     }
     ```

   - **Primaire knop** (`.primary-btn`):
     - Donkerrode achtergrond, die bij hover verandert in een accentkleur.
     ```css
     .primary-btn {
         background-color: var(--darkred);
     }

     .primary-btn:hover {
         background-color: var(--accentred);
     }
     ```

   - **Zoekknop** (`.search-btn`):
     - Accentrode achtergrond met donkerrode tekst.
     ```css
     .search-btn {
         background-color: var(--accentred);
         color: var(--darkred);
     }
     ```

---

### **Toepassing in de HTML**

Voorbeelden van het gebruik in HTML:

- **Typografie**:
   ```html
   <h1>Welkom op de website</h1>
   <h2>Over Ons</h2>
   <p>Deze website is ontworpen met een focus op toegankelijkheid en consistentie.</p>
   ```

- **Knoppen**:
   ```html
   <button class="cta-btn">Start Nu</button>
   <button class="primary-btn">Meer Informatie</button>
   <button class="search-btn">Zoeken</button>
   ```

- **Links**:
   ```html
   <a href="#contact">Contacteer ons</a>
   ```

---

### **Conclusie**

Deze styleguide helpt bij het creëren van een consistent en visueel aantrekkelijk ontwerp dat eenvoudig kan worden onderhouden en uitgebreid. Door het gebruik van CSS-variabelen, goed gedefinieerde typografie en modulaire componenten kan de styleguide effectief bijdragen aan een gestructureerde ontwikkeling.



