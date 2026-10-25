# Prvi koraci u terminalu

<!-- Ovo je početna verzija (v0) za projekt P1.
     Sve što je u [uglatim zagradama] zamijenite svojim tekstom.
     Očekivane rezultate prepišite sa SVOJEG zaslona, ne izmišljajte ih.
     Kad završite, ovaj komentar izbrišite. -->

[Jedna ili dvije rečenice: što će čitatelj naučiti u ovom tutorialu i koliko otprilike traje.]

## Prije početka

- Na kojem operacijskom sustavu i u kojem terminalu radite? Windows 11 i Git Bash.
- Visual Studio Code je pokrenut, a u njemu je otvorena mapa [atp-prirucnik].

## 1. Otvorite terminal

U izborniku **Terminal** odaberite **New Terminal**.

**Očekivani rezultat:** [Kako izgleda redak u kojem treperi pokazivač? Prepišite ga sa svojeg zaslona.]
ARAGORN@Argonath MINGW64 ~/Documents/atp-prirucnik (main)
$

## 2. Provjerite gdje se nalazite

```bash
pwd
```

**Očekivani rezultat:** /c/Users/ARAGORN/Documents/atp-prirucnik

## 3. Napravite mapu i uđite u nju

```bash
mkdir proba-terminala
cd proba-terminala
pwd
```

**Očekivani rezultat:** /c/Users/ARAGORN/Documents/atp-prirucnik/proba-terminala

## 4. Napravite datoteku i upišite u nju tekst

```bash
echo "# Moje bilješke" > biljeske.md
cat biljeske.md
```

**Očekivani rezultat:** # Moje bilješke

## 5. Dodajte još jedan redak

```bash
echo "- Naredba pwd ispisuje gdje se nalazim." >> biljeske.md
cat biljeske.md
```

**Očekivani rezultat:** # Moje bilješke
- Naredba pwd ispisuje gdje se nalazim.

Operator > služi za spremanje ili prepisivanje izlaza naredbe u datoteku, pri čemu se njen stari sadržaj briše. S druge strane, operator >> dodaje izlaz naredbe na kraj postojeće datoteke, čuvajući pritom sve njezine ranije podatke.

## 6. Kopirajte, preimenujte i izbrišite datoteku

```bash
cp biljeske.md kopija.md
mv kopija.md stara.md
rm stara.md
ls
```

**Očekivani rezultat:** biljeske.md

rm trajno briše datoteku

## Ako ne radi

| Poruka | Što znači | Što učiniti |
|---|---|---|
| `No such file or directory` | nema takve datoteke ili direktorija | potražiti drugdje |
| [Druga poruka koju ste vidjeli na vježbama] | [Objasnite.] | [Objasnite.] |

## Što dalje

Pogledajte priručnik Srca *Uvod u Linux*, poglavlja 2 i 3.
