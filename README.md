# Bionetic — Landing Page (Wariant 3)

---

## 🇵🇱 Wersja polska

### Opis projektu

Statyczna strona docelowa marki **Bionetic** — biokompleks do pielęgnacji
włosów, sprzedawany na rynku łotewskim. Wariant **3** to trzecie ujęcie
wizualne tego samego brandu: ciemne wino + złoto + blush, nowa typografia
i nowy układ sekcji — wyraźnie odróżniający się od wariantów 1 i 2.

Strona w całości w języku łotewskim. Treść, ceny i adresy dostosowane do
rynku Łotwy (Galleria Rīga, Ryga).

### Specyfikacja techniczna

| Element             | Wartość                                                       |
|---------------------|---------------------------------------------------------------|
| Język interfejsu    | Łotewski (`lang="lv"`)                                        |
| Stos technologiczny | HTML5, CSS3 (custom properties, Grid, Flexbox), vanilla JS    |
| Typografia          | Crimson Pro (serif) + Outfit (sans)                           |
| Paleta              | Deep wine (`#4a1f2e`) + Gold (`#c8965a`) + Blush (`#d6a596`)  |
| Ikony               | Font Awesome 6.5.1 (CDN)                                      |
| Wymagania serwera   | Brak — statyczne pliki                                        |

### Co wyróżnia wariant 3

- **Karta produktu w układzie plakatowym** (pionowym), w centrum sekcji
- **Sekcja kategorii** — 3 kafelki linkujące do innych sekcji
- **Sześć okrągłych ikon składników** zamiast naprzemiennych rzędów
- **Karta abonamentu** (jednorazowy zakup vs subskrypcja co 6 tygodni)
- **Cytaty w stylu redakcyjnym** (single quote) zamiast siatki opinii
- **Siatka UGC / Instagram** (6 zdjęć stylu życia)
- **Sekcja sklepu stacjonarnego** (store locator) z adresem i godzinami
- **Logo po lewej**, nawigacja na środku, ikony po prawej (jeszcze inny
  układ niż w wariancie 1 i 2)

### Funkcjonalność

- Sticky header z efektem scroll
- Menu mobilne (slide-in drawer)
- Koszyk z trwałym `localStorage` (klucz `bionetic_cart_v3`)
- Modal wyszukiwania z live-filtrowaniem
- Modal konta (logowanie / rejestracja, demo)
- Akordeon FAQ
- Pełnoekranowe polityki (Privacy, Terms, Delivery, Refund) z routingiem URL (`?page=...`)
- Walidacja formularza kontaktowego (JS)
- Formularz newslettera
- Baner cookie z trwałą zgodą (`bionetic_cookie_ok_v3`)
- Obsługa subskrypcji jako oddzielnej pozycji w koszyku (€34 vs €39)

### SEO

- Meta description, canonical, OpenGraph
- JSON-LD `LocalBusiness` z adresem Galleria Rīga
- Semantyczny HTML, atrybuty `alt` na obrazach
- `theme-color` dla mobilnych przeglądarek

### Struktura katalogu

```
├── index.html
├── css/
│   ├── base.css         (tokeny, reset, typografia, przyciski)
│   ├── components.css   (header, footer, modal, drawer, formularze, polityki)
│   └── sections.css     (hero, trust, produkt, kategorie, editorial,
│                         składniki, subskrypcja, founder, opinie, UGC,
│                         before/after, FAQ, sklep, kontakt, newsletter,
│                         responsive)
└── js/
    ├── cart.js          (koszyk + publiczne API window.BioneticCart)
    ├── ui.js            (header, menu, modale, FAQ, polityki, cookies, Esc)
    └── main.js          (search, walidacja kontaktu, newsletter, konto demo)
```

### Uruchomienie lokalne

To statyczna strona — wystarczy otworzyć `index.html` w przeglądarce lub
serwować dowolnym serwerem statycznym

### Responsywność

Punkty graniczne: **1024 px**, **768 px**, **480 px**. Strona została
zweryfikowana na typowych szerokościach mobile (360 px+), tablet i desktop.

### Status projektu

✅ **Wersja 1.0.0 — gotowa do wdrożenia produkcyjnego.**

### Polityka repozytorium

Niniejsze repozytorium publiczne zawiera **wyłącznie dokumentację oraz
zrzuty ekranu** mające potwierdzić wykonanie zlecenia (do celów rozliczeniowych
i podatkowych JDG).

Kompletny kod źródłowy znajduje się w **prywatnym repozytorium**, do którego
zleceniodawca otrzymuje bezpośredni dostęp w ramach przekazania projektu.
Szczegóły — w pliku `DELIVERY.md`.

---

## 🇬🇧 English version

### Project overview

A static landing page for the **Bionetic** brand — a biocomplex for hair care,
sold on the Latvian market. Variant **3** is the third visual treatment of the
same brand: deep wine + gold + blush, new typography and a new section
layout — clearly distinct from variants 1 and 2.

The page is fully in Latvian. All content, prices and addresses are tailored
to the Latvian market (Galleria Rīga, Riga).

### Technical specification

| Item             | Value                                                            |
|------------------|------------------------------------------------------------------|
| Interface lang   | Latvian (`lang="lv"`)                                            |
| Stack            | HTML5, CSS3 (custom properties, Grid, Flexbox), vanilla JS       |
| Typography       | Crimson Pro (serif) + Outfit (sans)                              |
| Palette          | Deep wine (`#4a1f2e`) + Gold (`#c8965a`) + Blush (`#d6a596`)     |
| Icons            | Font Awesome 6.5.1 (CDN)                                         |
| Server reqs      | None — static files                                              |

### What makes variant 3 distinct

- **Product card in a poster layout** (vertical), centered in the section
- **Categories section** — 3 tiles linking to other sections
- **Six circular ingredient icons** instead of alternating rows
- **Subscription card** (one-off vs every-6-weeks subscription)
- **Editorial-style quotes** (single quote) instead of a review grid
- **UGC / Instagram grid** (6 lifestyle photos)
- **Physical store section** (store locator) with address and hours
- **Logo left**, nav center, icons right (a third header layout, different
  from variants 1 and 2)

### Functionality

- Sticky header with scroll behavior
- Mobile menu (slide-in drawer)
- Cart persisted in `localStorage` (`bionetic_cart_v3`)
- Search modal with live filtering
- Account modal (login / register, demo)
- FAQ accordion
- Fullscreen policy overlays (Privacy, Terms, Delivery, Refund) with URL routing (`?page=...`)
- Contact form validation (JS)
- Newsletter form
- Cookie banner with persistent consent (`bionetic_cookie_ok_v3`)
- Subscription handled as a separate cart line (€34 vs €39)

### SEO

- Meta description, canonical, OpenGraph
- JSON-LD `LocalBusiness` with Galleria Rīga address
- Semantic HTML, `alt` on all images
- `theme-color` for mobile browsers

### Directory structure

```
site3/
├── index.html
├── css/
│   ├── base.css         (tokens, reset, typography, buttons)
│   ├── components.css   (header, footer, modal, drawer, forms, policies)
│   └── sections.css     (hero, trust, product, categories, editorial,
│                         ingredients, subscription, founder, reviews, UGC,
│                         before/after, FAQ, store, contact, newsletter,
│                         responsive)
└── js/
    ├── cart.js          (cart + public window.BioneticCart API)
    ├── ui.js            (header, menu, modals, FAQ, policies, cookies, Esc)
    └── main.js          (search, contact validation, newsletter, account demo)
```

### Running locally

This is a static page — open `index.html` directly or serve it with any
static server

### Responsiveness

Breakpoints: **1024 px**, **768 px**, **480 px**. Verified across typical
mobile (360 px+), tablet and desktop widths.

### Project status

✅ **Version 1.0.0 — production ready.**

### Repository policy

This public repository contains **only documentation and screenshots** that
prove the work was completed (used for invoicing and tax-reporting purposes
of the contractor's sole-proprietorship).

The complete source code lives in a **private repository** to which the client
receives direct access as part of project delivery. See `DELIVERY.md` for
details.
