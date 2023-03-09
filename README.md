# Heidegger Sigel

**Sigel** *n* (genitive Sigels, plural Sigel)  
: (linguistics, stenography) siglum, a conventional abbreviation for a word or words[^1]

Deze vergaarplaats \[*repository*\] bevat gegevens en hulpmiddelen om te werken met de afkortingen naar Heideggers werken.

[^1]: Wiktionary contributors, 'Sigel', Wiktionary, The Free Dictionary, 18 February 2023, 06:29 UTC, <https://en.wiktionary.org/w/index.php?title=Sigel&oldid=71322295> [accessed 9 March 2023] 

## Afkortingen

[Zie hier mijn voorgestelde afkortingen.](Sigel.md)

## Database van verschillende verwijzingen

Om in kaart te brengen wat de verschillende afkortingen zijn die gebruikt worden voor werken leg ik een database aan. Deze database bevat verschillende onderdelen:

- Een bibliografie met werken die naar Heideggers werken verwijzen.
- Een bibliografie van verschillende uitgaven van Heideggers werken. Which is an export of https://www.zotero.org/groups/4982216/martin_heidegger_gesamtausgabe/
- Een database die een verbinding legt tussen de twee, met de gebruikte afkortingen.

### Datamodel

Het datamodel de eerste twee is CSL YAML. De laatste database volgt het volgende datamodel:
```yaml
citekey_sec_literature:
  abbreviations:
    - citekey_pr_literature: abbrev.
```

### Citekeys

De citekeys voor de verschillende uitgaven moeten uniek zijn en worden aan de hand van de volgende formule gevormd: `auth.lower + shorttitle(3,3) + year` (dit is de standaard voor Zotero's ‘Better BibTeX’ plugin.)
