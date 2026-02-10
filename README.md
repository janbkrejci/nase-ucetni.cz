# Naše Účetní - Rozcestník prezentací

Tento projekt slouží jako jednoduchý, vizuálně přehledný rozcestník pro studenty a zájemce o účetnictví. Obsahuje odkazy na prezentace a výukové materiály (převážně uložené na OneDrive/SharePointu).

Web běží na adrese [nase-ucetni.cz](https://nase-ucetni.cz).

## Jak přidat novou prezentaci

Obsah webu je definován přímo v souboru `index.html` pomocí JavaScriptového pole `resources`. Pro přidání nového odkazu postupujte následovně:

1. Otevřete soubor `index.html`.
2. Najděte sekci `// --- DATA ---` (kolem řádku 38).
3. Do pole `const resources = [...]` přidejte nový objekt ve formátu:

```javascript
{
    title: "Název vaší prezentace",
    description: "Stručný popis toho, co se v prezentaci nachází",
    type: "presentation", // určuje ikonu a barvu (aktuálně podporováno: 'presentation')
    category: "Název kategorie", // např. 'Účetnictví pro pokročilé'
    url: "https://odkaz-na-vasi-prezentaci.com"
}
```

4. Uložte soubor. Změny se po nahrání na server (nebo commitu do repozitáře) okamžitě projeví.

## Technické detaily

- **Frontend:** Čisté HTML se stylováním přes [Tailwind CSS](https://tailwindcss.com) (načítáno přes CDN).
- **Ikony:** SVG ikony vložené přímo v konfiguraci `typeConfig`.
- **Hosting:** Projekt je nastaven pro statický hosting (např. GitHub Pages) s vlastní doménou definovanou v souboru `CNAME`.

## Kontakt

V případě dotazů nebo potřeby technické pomoci kontaktujte:
[jaroslava.krejci@tailorservices.com](mailto:jaroslava.krejci@tailorservices.com)
