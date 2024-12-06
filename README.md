# Styleguide

Ontwerp en maak met een team een styleguide om te gebruiken voor een opdracht van een opdrachtgever.
![Schermafbeelding 2024-11-15 094435](https://github.com/user-attachments/assets/f12f05be-b6c1-4c98-b75f-3290959d8f1c)

![Schermafbeelding 2024-11-15 094446](https://github.com/user-attachments/assets/23ed62cf-57bd-4381-a77f-2fb8c6fddeb6)

![Schermafbeelding 2024-11-15 094524](https://github.com/user-attachments/assets/4b44bb43-ca1e-4070-8820-ebddf074a3f5)

Het lijkt erop dat je een uitgebreide CSS-code hebt die een aantal stijlen definieert voor een website, inclusief kleurvariabelen, typografie, knoppen en invoerelementen. Als je wilt dat ik de `README` bijwerk op basis van deze nieuwe code, kan ik dit als volgt doen:

---

# README: Styleguide Documentatie

Deze readme beschrijft hoe we de CSS-code in de styleguide hebben opgebouwd. Het doel is om consistentie, schaalbaarheid en toegankelijkheid te waarborgen, met een focus op flexibele stijlen voor knoppen, tekst, en invoerelementen.

---

## Wat staat er in deze styleguide?

1. **Globale CSS-instellingen**
2. **CSS-variabelen (Kleuren en Lettertypen)**
3. **Typografie**
4. **Knoppen en Links**
5. **Invoerelementen**
6. **Voorbeelden in HTML**

---

### 1. Globale CSS-instellingen

De algemene instellingen zijn bedoeld om ervoor te zorgen dat alles consistent wordt weergegeven op de website:

```css
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
```

- **`margin` en `padding`:** Alle elementen beginnen zonder extra marges of padding.
- **`box-sizing: border-box`:** Dit zorgt ervoor dat padding en borders worden meegerekend in de totale afmetingen van de elementen.

---

### 2. CSS-variabelen (Kleuren en Lettertypen)

We gebruiken CSS-variabelen voor consistente kleuren, lettertypen en andere stijlen. Dit maakt de code gemakkelijker te onderhouden en aan te passen.

**Kleuren:**

```css
--darkred: #6A0025;
--accentred: #6a002580;
--white: #FFF;
--lightred: #F0E5E9;
--black: #1F000B;
```

**Lettertypen:**

```css
--vag-rund: Arial, Helvetica, sans-serif;
--open-sans: "Open Sans";
```

**Lettergroottes:**

```css
--font-size-xl: 45px;
--font-size-l: 35px;
--font-size-m: 20px;
--font-size-s: 18px;
```

**Lettergewichten:**

```css
--light: 400;
--normal: 500;
--bold: 600;
```

- **Waarom deze keuzes?** We hebben kleuren gekozen die een sterk contrast bieden voor toegankelijkheid. Lettertypen zijn gemakkelijk leesbaar en geschikt voor webgebruik.

---

### 3. Typografie

De stijlen voor koppen en tekst zorgen voor een duidelijke hiërarchie en leesbaarheid.

```css
h1 {
    font-size: var(--font-size-xl);
    color: var(--darkred);
}

h2 {
    font-size: var(--font-size-l);
    padding-bottom: 30px;
    color: var(--darkred);
}

h3 {
    font-size: var(--font-size-m);
}
```

- **Waarom?** Koppen hebben grotere formaten en een sterk contrast om ze op te laten vallen. Subkoppen en kleinere koppen gebruiken een afgeleide stijl voor consistentie.

---

### 4. Knoppen en Links

Knoppen en links zijn belangrijk voor interactie met de website. De stijlen zijn eenvoudig maar effectief en verbeteren de gebruikerservaring.

**Algemene knop:**

```css
button {
    padding: 15px 40px;
    background-color: var(--darkred);
    color: var(--white);
    align-items: center;
    border: none;
    border-radius: 10px;
}
```

**Call-to-action knop:**

```css
.cta-btn {
    background-color: var(--black); 
}

.cta-btn:hover {
    background-color: var(--lightred);
    color: var(--black);
}
```

**Primaire knop:**

```css
.primary-btn {
    background-color: var(--darkred);
}

.primary-btn:hover {
    background-color: var(--accentred);
}
```

- **Waarom?** De knoppen zijn goed zichtbaar, met kleurveranderingen op hover om gebruikers duidelijk te maken dat ze interactief zijn.

---

### 5. Invoerelementen

Invoerelementen zoals zoekvelden en knoppen zijn gestyled voor consistentie en toegankelijkheid.

```css
input[type="button"] {
    padding: 10px 20px;
    border: none;
    background-color: var(--darkred, #6A0025);
}

input[type="button"]:checked {
    background-color: var(--accentred);
}
```

**Zoekveld:**

```css
input[type="search"], input[type="search"]:focus {
    width: 100%;
    height: 3rem;
    padding: 1.5rem;
    margin: 1rem 0;
    border: none;
    outline: none;
    background-color: var(--white);
}
```

- **Waarom?** Zoekvelden zijn breder en beter zichtbaar, met een duidelijk focusgedrag voor een betere gebruikerservaring.

---

### 6. Voorbeelden in HTML

Met de stijlen uit de styleguide kun je eenvoudig elementen creëren die consistent en toegankelijk zijn.

**Typografie:**

```html
<h1>Welkom op onze website</h1>
<h2>Onze Diensten</h2>
<p>Wij bieden uitstekende webontwikkeling, gericht op prestaties en toegankelijkheid.</p>
```

**Knoppen:**

```html
<button class="cta-btn">Start Nu</button>
<button class="primary-btn">Meer Informatie</button>
```

**Links:**

```html
<a href="#contact">Neem contact met ons op</a>
```

---

### Conclusie

Deze styleguide biedt een gestructureerde manier om consistente en toegankelijke websites te bouwen. Door gebruik te maken van CSS-variabelen en gestandaardiseerde stijlen voor knoppen, invoerelementen en typografie, kunnen we een gebruiksvriendelijke en flexibele gebruikersinterface creëren die gemakkelijk te onderhouden is.



