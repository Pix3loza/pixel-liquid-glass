# Pixel Liquid Glass

Zestaw lekkich, modularnych efektów "liquid glass" (glassmorphism + płynna refrakcja + blob + ripple + dripping + kondensacja + shimmer) w czystym CSS i Vanilla JS.

## Funkcje
- Glassmorphism + dynamiczne rozmycie / gradienty
- Ripple (klik / pointer)
- Morphing blob (płynny kształt tła)
- Drip border (animujące się “spływające” krawędzie)
- Shimmer highlight (szklany refleks przesuwający się po powierzchni)
- Condensation particles (drobne kropelki / parowanie)
- Tilt / parallax (reakcja na ruch kursora / device orientation)
- Custom Elements (`<liquid-glass-card>`, `<liquid-glass-blob>`)
- Autoinicjalizacja przez `data-liquid-*`
- Brak zależności zewnętrznych
- Możliwość łatwego tree-shake (modularna struktura)
- Działa w trybie degradacji (fallback dla braku `backdrop-filter`)

## Szybki start

HTML minimal:

```html
<link rel="stylesheet" href="dist/liquid-glass.min.css" />
<script type="module" src="dist/liquid-glass.min.js"></script>

<div class="lg-card" data-liquid="ripple shimmer particles">
  <h2>Pixel Liquid Glass</h2>
  <p>Przykładowy efekt.</p>
</div>
```

Albo przez Custom Element:
```html
<liquid-glass-card effects="ripple shimmer tilt">
  <h3>Tytuł</h3>
</liquid-glass-card>
```

## Atrybuty
- `data-liquid="ripple shimmer blob tilt drip particles"`
- `data-liquid-intensity="0.2"` (uniwersalne — różny sens w różnych efektach)
- `effects="..."` w custom elements (analogiczne)

## Dostępne klasy bazowe
- `.lg-root` (opcjonalny kontener)
- `.lg-card`
- `.lg-blob`
- `.lg-drip`
- `.lg-overlay` (wewnętrzne)
- `.lg-particles-layer`

## Podgląd
Zobacz: `examples/index.html` (pełny) oraz `examples/minimal.html`.

## Build / Development
Skrypt prosty: `node scripts/build.js` generuje pliki w `dist/`.
Możesz edytować w `src/` i przebudować.

## Licencja
MIT – patrz [LICENSE](LICENSE).

## Spis treści dokumentacji
- [USAGE](docs/USAGE.md)
- [ARCHITECTURE](docs/ARCHITECTURE.md)

Miłej zabawy!