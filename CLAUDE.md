# CLAUDE.md

This file provides guidance to Claude Code when working with this project.

## Role

Du agierst als Senior Full-Stack Webentwickler und UI/UX Designer mit über 10 Jahren Erfahrungen Projektmanagement und 7-stelligen Budgetverantwortung. Dein Ziel ist es, eine moderne, performante und responsive Website auf Basis der folgenden Spezifikationen zu erstellen.

---

## Context & Project Scope

- **Projektname:** Pochat Automobile Baden-Baden
- **Zielgruppe:** Liebhaber, Sammler und Käufer exklusiver Gebrauchtwagen, wie Sportwagen, Luxusautos und Premiumfahrzeuge
- **Kernbotschaft/Ziel:** Faszination, Sportlichkeit, Exklusivität, Emotionalität und der Verkauf von Premiumfahrzeugen.
- **Domain:** https://www.pochat-automobile.de/
- **Produkt:** Exklusive Fahrzeuge, wie Sportwagen und Luxusautos. Gebrauchtwagen, Neufahrzeuge, Oldtimer, Youngtimer, Jahreswagen - alle im Bestzustand.
- **Inhaber:** Werner Pochat (Geschäftsführer, Kraftfahrzeugmeister und Dipl. Betriebswirt)

---

## Technical Stack

- **Frontend:** HTML5, CSS3 (Tailwind CSS via CDN) und Vanilla JavaScript
- **Icons:** Font Awesome (via CDN)
- **Fonts:** Inter (300-800) via Google Fonts
- **Newsletter:** Mailchimp (TODO)
- **Kontaktformular:** Inline JavaScript (Formular-Handler implementiert)
- **Payment:** Stripe (optional)

---

## Hosting & Deployment

- **Staging:** Netlify
- **Production:** noch unbekannt
- **Repository:** GitHub - https://github.com/MacCoy69/pochat-automobile.git

### Git Workflow
```
1. Local Development → Browser Preview
2. Git Commit nach jedem Feature
3. Staging-Branch → Netlify Preview
4. Production-Branch (main) → All-Inkl. Live
```

---

## Design Specifications

### Farbschema (Tailwind Custom Colors)
```css
dark: #080706       /* Primary Dark / Background */
light: #efefef      /* Light Background */
accent: #d1b280     /* Gold/Bronze Accent */
accent2: #594d46    /* Secondary Brown */
white: #ffffff      /* White */
```

### Typografie
- **Font:** Inter (300, 400, 500, 600, 700, 800)
- **Verwendung:** `font-sans: ['Inter', 'sans-serif']`

### Logo
- Text-basiertes Logo: `Wunderwald<span class="text-accent font-light">Media</span>`
- Style: Bold "Wunderwald" + Light Gold "Media"

### Vorhandene Bilder (./images/)
```
marco-wunderwald.jpg          # Profilbild für "Über mich" Section
wunderwald-media-bg.png       # Hero Background Image
```

### Design-Patterns (implementiert)
- **Gradient Hero:** `linear-gradient(135deg, #080706 0%, #1a1816 50%, #0d0c0b 100%)`
- **Chat Animation:** Simulierter ChatGPT-Dialog im Hero
- **Glassmorphism:** Navigation mit `backdrop-blur-lg`
- **Fade-Up Animations:** Scroll-triggered Animationen
- **Stat Bars:** Animierte Fortschrittsbalken
- **FAQ Accordion:** Expand/Collapse mit Schema.org Markup
- **Modal System:** Für Impressum/Datenschutz

---

## Seitenstruktur (Single Page Application)

### Implementierte Sections
| Section | ID | Status |
|---------|-----|--------|
| Navigation | `#navbar` | ✅ Fertig |
| Hero | `#start` | ✅ Fertig (mit Chat-Animation) |
| Problem | `#problem` | ✅ Fertig |
| Was ist GEO | `#was-ist-geo` | ✅ Fertig |
| Statistiken | - | ✅ Fertig (animierte Bars) |
| Leistungen | `#leistungen` | ✅ Fertig |
| Preise | `#preise` | ✅ Fertig |
| Testimonials | - | ✅ Fertig (Platzhalter) |
| Referenzen | `#referenzen` | ✅ Fertig (6 Projekte) |
| FAQ | `#faq` | ✅ Fertig (5 FAQs mit Schema.org) |
| Über mich | - | ✅ Fertig |
| CTA | - | ✅ Fertig |
| Kontakt | `#kontakt` | ✅ Fertig |
| Footer | - | ✅ Fertig |

### Modals
- `#impressum-modal` - ✅ Fertig (Basic)
- `#datenschutz-modal` - ✅ Fertig (Basic)

---

## Produkte & Preise

### 1. Starter - €990
- AI Readiness Check (ChatGPT, Perplexity, Google AI)
- Prompt-Recherche für Ihre Branche
- FAQ-Sektion erstellt & implementiert
- Handlungsreport
- 30 Min. Strategiegespräch
- Optional: Wettbewerber-Analyse (+€200)

### 2. Professional - €1.990 (Empfohlen)
- Alles aus Starter
- Komplette On-Site GEO Optimierung
- Schema.org Markup implementiert
- Content-Anreicherung (Statistiken, Quellen)
- Technische Optimierung
- Optional: Monitoring (+€290/Monat)

### 3. Premium - €4.990
- Alles aus Professional
- Off-Site GEO Strategie & Setup
- LinkedIn/Branchen-Content
- Review-Strategie
- 3 Monate Monitoring inklusive
- Prioritäts-Support

---

## Leistungen

1. **GEO Audit**
   - AI Readiness Score
   - Prompt-Recherche
   - FAQ-Sektion erstellt

2. **GEO Umsetzung**
   - Schema.org implementiert
   - Content optimiert
   - Technische Optimierung

3. **AI-Ready Webdesign**
   - Mobile First
   - GEO von Tag 1
   - Conversion optimiert

---

## Implementierte Features

### Navigation
- ✅ Fixed Navigation mit Backdrop-Blur
- ✅ Desktop Navigation mit Links
- ✅ Mobile Menu (Slide-in)
- ✅ CTA Button "Kostenlose Analyse"

### Hero Section
- ✅ Background Image mit Dark Overlay
- ✅ Animated ChatGPT Simulation
- ✅ Trust Badges (25+ Jahre, 100% Umsetzung, AI Master 2025)
- ✅ Dual CTA Buttons

### Interactive Elements
- ✅ Chat Animation (3 rotierende Dialoge)
- ✅ FAQ Accordion mit Schema.org
- ✅ Animated Stat Bars (Scroll-triggered)
- ✅ Fade-Up Animations
- ✅ Modal System
- ✅ Contact Form

### Footer
- ✅ 4-Spalten-Layout
- ✅ Navigation Links
- ✅ Rechtliche Links (Modal-Trigger)
- ✅ Copyright

---

## Referenz-Projekte (implementiert)

1. Deutsche Sporteltern - deutschesporteltern.de
2. Mastro Olivenöl - mastro-olivenoel.de
3. OxyGym - oxygym.de
4. Aloka Yoga - aloka-yoga.com
5. Medienwerk BAD - medienwerk-bad.de
6. Rheia Group - rheia-group.com

---

## SEO & GEO Status

### Implementiert
- ✅ Meta Title & Description
- ✅ Schema.org FAQPage Markup
- ✅ Schema.org LocalBusiness Markup
- ✅ Semantic HTML
- ✅ Smooth Scroll
- ✅ Mobile Responsive

### GEO-Optimiert
- ✅ FAQ mit Statistiken und Quellen
- ✅ Klare Frage-Antwort-Struktur
- ✅ Zitierbare Zahlen (40%, 527%, 4.4×, etc.)
- ✅ Quellenangaben (Princeton/Georgia Tech, Sequencr.ai, etc.)

---

## Offene TODOs

### Hohe Priorität
- [ ] Testimonials mit echten Kundendaten ersetzen
- [ ] Impressum vervollständigen
- [ ] Datenschutzerklärung vervollständigen
- [ ] Kontaktformular Backend (FormSubmit oder eigenes Backend)

### Mittlere Priorität
- [ ] Newsletter-Integration (Mailchimp)
- [ ] Cookie Consent Banner (DSGVO)
- [ ] Echte Projekt-Screenshots statt Unsplash
- [ ] Google Analytics / Tag Manager

### Niedrige Priorität
- [ ] Weitere FAQ hinzufügen
- [ ] Blog-Section
- [ ] Case Studies Page
- [ ] Bilder zu WebP konvertieren

---

## Project Structure

```
www/
├── images/
│   ├── marco-wunderwald.jpg
│   └── wunderwald-media-bg.png
├── index.html                 # ✅ Single Page Website
└── claude.md                  # Diese Datei
```

---

## Kontaktdaten

- **Name:** Marco Wunderwald
- **Firma:** Wunderwald Media
- **Adresse:** Pestalozziweg 13, 76530 Baden-Baden
- **Telefon:** +49 172 7383860
- **E-Mail:** mw@wunderwald-media.de

---

## Code-Referenz (index.html)

### Tailwind Config (Zeile 14-29)
Custom Colors und Font-Family definiert.

### CSS Klassen (Zeile 32-144)
- `.gradient-hero` - Hero Background Gradient
- `.chat-container` - ChatGPT Simulation Container
- `.typing-cursor` - Typing Animation
- `.chat-message` - Chat Bubble Animation
- `.fade-up` - Scroll Animation
- `.faq-answer` - FAQ Accordion
- `.stat-bar` - Animated Progress Bars
- `.testimonial-card` - Hover Effects
- `.project-card` - Portfolio Hover
- `.modal` - Modal System
- `.glow` - Box Shadow Effect

### JavaScript Funktionen (ab Zeile 1203)
- `toggleMenu()` - Mobile Menu
- `typeText()` - Typing Animation
- `runChatAnimation()` - Chat Simulation Loop
- `toggleFaq()` - FAQ Accordion
- `openModal()` / `closeModal()` - Modal Control
- `submitForm()` - Contact Form Handler
- IntersectionObserver für Scroll-Animationen

### Schema.org (ab Zeile 1363)
- LocalBusiness Markup
- FAQPage Markup (inline bei FAQ Section)

---

## Wichtige Hinweise

1. **Single Page:** Alles in einer index.html (keine Unterseiten)
2. **Bildpfade:** Lokale Bilder in `images/` mit Fallback zu `wunderwald.media`
3. **Tailwind via CDN:** Keine Build-Tools notwendig
4. **Testimonials:** Aktuell Platzhalter `[Kundenname]` - müssen ersetzt werden
5. **Formular:** Simuliert Absenden - Backend fehlt noch
6. **Email-Schutz:** Cloudflare Email Protection aktiv
