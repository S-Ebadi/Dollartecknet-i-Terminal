# Innehållsförteckning

1. [Dollartecknet – Minimal och ren terminalprompt](#1-dollartecknet--minimal-och-ren-terminalprompt-på-macos)
2. [psutil – Visa CPU-användning i Python](#2-psutil--cpu-användning-med-psutil)


# 1. Dollartecknet – Minimal och ren terminalprompt på macOS

Följ dessa steg för att göra din terminalprompt så enkel som möjligt – endast ett dollartecken ($) visas, utan användarnamn, värdnamn eller sökväg. Perfekt för en ren och fokuserad terminal!

---

## Steg-för-steg: Minimal bash-prompt
...existing code...


# 2. psutil – CPU-användning med psutil

Detta projekt visar hur du installerar och använder Python-biblioteket `psutil` för att läsa av CPU-användningen på din dator.

---

## Steg-för-steg-guide (macOS & py-friendly)
...existing code...




# CPU-användning med psutil

Detta projekt visar hur du installerar och använder Python-biblioteket `psutil` för att läsa av CPU-användningen på din dator.

---

## Steg-för-steg-guide (macOS & py-friendly)

### 1. Klona eller ladda ner projektet

Ladda ner eller klona denna mapp till din dator.

### 2. Skapa och aktivera en virtuell miljö (valfritt men rekommenderas)

Öppna Terminalen i projektmappen och kör:

```bash
python3 -m venv .venv
source .venv/bin/activate
```

### 3. Installera beroenden

Installera nödvändiga Python-paket med:

```bash
pip install -r requirements.txt
```

### 4. Kontrollera att `psutil` är installerat

Kör i terminalen:

```bash
pip show psutil
```

Du ska se information om psutil-paketet.

### 5. Kör CPU-exemplet

Kör Python-filen som visar CPU-användningen:

```bash
python cpu_usage.py
```

Du får då ut aktuell CPU-användning i procent.

---

## Felsökning

- Om du får fel om att `psutil` saknas, kontrollera att du är i rätt miljö och att installationen lyckades.
- Om du får "Permission denied", kontrollera att du har rättigheter till mappen.
- Om du vill installera om alla paket, ta bort `.venv`-mappen och börja om från steg 2.

---

## Om du vill ändra koden

Redigera `cpu_usage.py` för att visa mer information eller göra fler mätningar.

---

"A true hero isn't measured by the size of his strength, but by the strength of his heart"
- Zeus
