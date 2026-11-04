# Prvi koraci s Pandocom

U ovom vodiču naučit ćete kako instalirati Pandoc i pretvoriti Markdown datoteku u Word dokument te HTML web-stranicu. Za prolazak kroz cijeli vodič potrebno vam je oko 10 minuta.

Provjereno s Pandocom 3.13 na Windowsu 11 i Git Bash terminalu.

## Prije početka

Instaliran uređivač teksta (npr. VS Code, Notepad++, Jet Brains)
Otvoren terminal (PowerShell / Command Prompt na Windowsu ili Terminal na Macu)
Pripremljena jednostavna Markdown datoteka (npr. README.md s nekoliko redaka teksta)

## 1. Instalirajte Pandoc

### Windows

Preuzmite službeni .zip paket s Pandoc GitHub Releases stranice.
Raspakirajte ZIP arhivu na lokalni disk (npr. C:\Pandoc).

Dodajte put do mape (putanja u kojoj se nalazi pandoc.exe) u varijablu okruženja PATH:

```
export PATH="/c/Users/username/pandoc-3.13-windows-x86_64/pandoc-3.13:$PATH"
```

## 2. Provjerite instalaciju

```bash
pandoc --version
```

**Očekivani rezultat:** pandoc 3.13

## 3. Pretvorite Markdown u Word

```
pandoc README.md -o izlaz/README.docx
```

Trebali bi u Wordu vidjeti kako su naslovi dobili odgovarajuće headinge u Wordu.

## 4. Pretvorite Markdown u web-stranicu

```
pandoc README.md -s -o izlaz/README-samostalno.html
```

Napravit će se cijela web-stranica (-s znači standalone)

## Ako ne radi

| Poruka | Što znači | Što učiniti |
|---|---|---|
| command not found ili 'pandoc' is not recognized...| Sustav ne može pronaći izvršnu datoteku Pandoca jer nije u PATH-u ili instalacija nije završena | Provjerite je li put do Pandoca dodan u sustavni PATH, pa zatvorite i ponovno otvorite terminal |
| cannot open file README.md | Terminal se ne nalazi u istoj mapi u kojoj je spremljena vaša Markdown datoteka | Navigirajte do prave mape pomoću naredbe cd put/do/mape ili navedite punu putanju do datoteke |

## Što ste napravili

Uspješno ste instalirali i konfigurirali Pandoc na svom računalu te provjerili njegov rad putem terminala. Sada znate kako iz jedne izvorne Markdown datoteke jednostavnim naredbama generirati Word dokument i samostalnu HTML web-stranicu, a ima i još formata koje pandoc podržava.
