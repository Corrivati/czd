# Editor homepage — CZECHDESIGN SHOP

Jednosouborový editor obsahu homepage. Vyplníte pole, nástroj vygeneruje
hotové HTML k vložení do administrace.

**Spustit:** https://corrivati.github.io/czd/

## Co umí

- Všechny sekce homepage: úvodní text, Oblíbené kategorie, Inspirace,
  Kampaně, Snoubení, Designéři a značky, O nás
- **Načíst aktuální HTML** — vložíte kód z administrace a nástroj z něj
  předvyplní všechna pole. Sekce, které v kódu nenajde, nechá beze změny
- Živý náhled ve stylu webu, záložky v náhledu fungují
- Kontrola před exportem: chybějící a duplicitní alt popisky, prázdné
  cesty k obrázkům, odkazy bez lomítka, nečíselná ID widgetů, kolidující
  kotvy
- Karty a designéři jsou sbalení, dají se přidávat, mazat, duplikovat
  a přesouvat
- Export: Kopírovat HTML, Stáhnout HTML, Uložit / Načíst JSON

## Práce s obsahem

Rozpracovaný obsah se nikam neukládá sám. Před zavřením karty použijte
**Uložit JSON** a příště **Načíst JSON**. Nebo si vždy načtěte aktuální
HTML z administrace a pracujte z něj.

## Úpravy

Celý nástroj je jeden soubor `index.html` bez závislostí. Uvnitř je
rozdělený na číslované sekce: výchozí obsah, generátor HTML, čtečka HTML,
kontrola, náhled, formulář, překreslení, akce.

Po commitu do `main` se změna projeví na Pages do zhruba minuty.
