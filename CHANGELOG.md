# Changelog — Bionetic Landing (Wariant 3)

> Format zgodny z [Keep a Changelog](https://keepachangelog.com/) ·
> projekt stosuje [Semantic Versioning](https://semver.org/).

---

## 🇵🇱 Wersja polska

### [1.0.0] — 2026-05-13

#### Dodane
- Pełna treść w języku łotewskim, dostosowana do rynku Łotwy.
- Nowa paleta: deep wine (`#4a1f2e`) + złoto (`#c8965a`) + blush (`#d6a596`)
  i krem — wyraźnie odróżniająca wariant 3 od wcześniejszych wariantów.
- Nowa typografia: Crimson Pro (serif) + Outfit (sans).
- Modularna struktura plików zgodna z wariantami 1 i 2 (osobne katalogi
  `css/` i `js/`).
- Sekcje: ogłoszenie, header (logo lewo / nawigacja środek / ikony prawo),
  hero (minimalny wycentrowany z dryfującym obrazem produktu),
  pasek zaufania, karta produktu w układzie plakatowym (pionowym),
  siatka kategorii (3 kafelki linkujące),
  blok redakcyjny (naprzemienne duży obraz + tekst),
  spotlight 6 składników w okrągłych ikonach,
  porównanie zakup jednorazowy vs abonement (€39 / €34),
  historia założycielki z dużym zdjęciem,
  ściana 4 cytatów w stylu redakcyjnym,
  siatka UGC / Instagram (6 zdjęć),
  before/after (2 obrazy z disclaimerem),
  FAQ, sklep stacjonarny (store locator) z godzinami,
  formularz kontaktowy, newsletter, footer.
- Koszyk z trwałym `localStorage` (klucz `bionetic_cart_v3`).
- Subskrypcja obsługiwana jako oddzielna pozycja w koszyku
  (`bionetic-sub`, €34/flakon co 6 tygodni).
- Modal wyszukiwania + modal konta (logowanie / rejestracja demo).
- Pełnoekranowe polityki (Privacy, Terms, Delivery, Refund) z routingiem
  URL (`?page=...`).
- Banner cookie z trwałą zgodą (`bionetic_cookie_ok_v3`).
- Walidacja JS dla formularza kontaktowego.
- SEO: meta description, canonical, OpenGraph, JSON-LD `LocalBusiness`
  z adresem Galleria Rīga, Ryga.
- Responsywność: punkty graniczne 1024 / 768 / 480 px, testowane od 360 px.
- Dokumentacja `README.md`, `CHANGELOG.md`, `DELIVERY.md` (PL + EN).

---

## 🇬🇧 English version

### [1.0.0] — 2026-05-13

#### Added
- Full content in Latvian, localized for the Latvian market.
- New palette: deep wine (`#4a1f2e`) + gold (`#c8965a`) + blush (`#d6a596`)
  and cream — clearly distinguishing variant 3 from earlier variants.
- New typography: Crimson Pro (serif) + Outfit (sans).
- Modular file structure matching variants 1 and 2 (separate `css/` and
  `js/` directories).
- Sections: announcement bar, header (logo left / nav center / icons right),
  hero (minimal centered with floating product image),
  trust strip, product card in a poster layout (vertical),
  categories grid (3 linking tiles),
  editorial block (alternating large image + text),
  6-ingredient spotlight in circular icons,
  one-off vs subscription comparison (€39 / €34),
  founder story with a large portrait,
  4-quote editorial review wall,
  UGC / Instagram grid (6 photos),
  before/after (2 images with disclaimer),
  FAQ, physical store section (store locator) with opening hours,
  contact form, newsletter, footer.
- Cart persisted in `localStorage` (`bionetic_cart_v3`).
- Subscription handled as a separate cart line item
  (`bionetic-sub`, €34/bottle every 6 weeks).
- Search modal + account modal (demo login / register).
- Fullscreen policy overlays (Privacy, Terms, Delivery, Refund) with URL
  routing (`?page=...`).
- Cookie banner with persistent consent (`bionetic_cookie_ok_v3`).
- JS validation on the contact form.
- SEO: meta description, canonical, OpenGraph, JSON-LD `LocalBusiness` with
  the Galleria Rīga, Riga address.
- Responsiveness: breakpoints at 1024 / 768 / 480 px, verified from 360 px.
- Documentation `README.md`, `CHANGELOG.md`, `DELIVERY.md` (PL + EN).
