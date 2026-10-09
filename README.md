# Editor homepage — CZECHDESIGN SHOP

Jednosouborový editor obsahu homepage. Vyplníte pole, nástroj vygeneruje
hotové HTML k vložení do administrace.

**Spustit:** https://corrivati.github.io/czd/

## Co umí

- Začíná se vždy vložením aktuálního HTML z administrace
  (**Vzhled a obsah → Titulní strana → Nástroje → Zdrojový kód**). Editor
  nemá žádný vlastní výchozí obsah, pracuje jen s tím, co mu dáte
- Sekce: úvodní text, Oblíbené kategorie, Inspirace, Kampaně, Snoubení,
  Designéři a značky, O nás. Vypíše se jen to, co bylo ve vloženém kódu,
  chybějící sekce nástroj vypíše jako upozornění
- Živý náhled ve stylu webu, záložky v náhledu fungují
- Kontrola před exportem: chybějící a duplicitní alt popisky, prázdné
  cesty k obrázkům, odkazy bez lomítka, nečíselná ID widgetů, kolidující
  kotvy
- Karty a designéři jsou sbalení, dají se přidávat, mazat, duplikovat
  a přesouvat
- Export: Kopírovat HTML
- Vestavěný **Návod** a **zálohy** starších verzí homepage

## Zálohy

Složka `zalohy/` drží starší verze homepage. Na úvodní obrazovce se
nabídnou pod tlačítkem „Nemáte kód po ruce?“.

Novou zálohu přidáte tak, že do `zalohy/` commitnete HTML soubor
a doplníte záznam do `zalohy/index.json`:

```json
{ "file": "2026-11-02-homepage.html", "date": "2. 11. 2026",
  "label": "Homepage po vánoční kampani", "note": "Krátký popis" }
```

Úplnou historii nese i samotný git, zálohy jsou jen to, co má být po ruce
přímo v nástroji.

## Práce s obsahem

Rozpracovaný obsah se nikam neukládá. Zavřením karty se ztratí, takže
hotový kód rovnou kopírujte do administrace. Příště zase začnete tím, že
si načtete aktuální HTML.

## Úpravy

Celý nástroj je jeden soubor `index.html` bez závislostí. Uvnitř je
rozdělený na číslované sekce: stav, generátor HTML, čtečka HTML,
kontrola, náhled, formulář, překreslení, akce.

Po commitu do `main` se změna projeví na Pages do zhruba minuty.
