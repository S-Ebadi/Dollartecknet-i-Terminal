
# Innehållsförteckning

1. [Dollartecknet – Minimal och ren terminalprompt](#1-dollartecknet--minimal-och-ren-terminalprompt-på-macos)
2. [psutil – CPU-användning i Python](#2-psutil--cpu-användning-med-psutil)

---

# 1. Dollartecknet – Minimal och ren terminalprompt på macOS

> **Syfte:** Få en ren terminalprompt med endast ett `$` – inget användarnamn, värdnamn eller sökväg. Perfekt för fokus och enkelhet!

## Steg-för-steg

**1. Öppna eller skapa din bash-profil**

```bash
nano ~/.bash_profile
```

**2. Lägg till följande rader:**

```bash
PS1='$ '
export BASH_SILENCE_DEPRECATION_WARNING=1
```

* `PS1='$ '` gör prompten till endast ett dollartecken.
* `export BASH_SILENCE_DEPRECATION_WARNING=1` döljer zsh-varningen på macOS.

Spara och avsluta (`Ctrl+O`, `Enter`, `Ctrl+X`).

**3. Ladda om profilen:**

```bash
source ~/.bash_profile
```

Prompten ska nu se ut så här:

```bash
$ 
```

**Felsökning:**

- Får du "No such file or directory"? Skapa filen enligt ovan.
- Vill du återställa? Ta bort eller kommentera raderna i `.bash_profile`.
- Guiden gäller bash. Använder du zsh eller annat skal är stegen annorlunda.

---

# 2. psutil – CPU-användning med psutil

> **Syfte:** Installera och använda Python-biblioteket `psutil` för att visa aktuell CPU-användning i terminalen.

## Steg-för-steg

**1. Klona eller ladda ner projektet**

Ladda ner eller klona denna mapp till din dator.

**2. Skapa och aktivera en virtuell miljö (rekommenderas):**

```bash
python3 -m venv .venv
source .venv/bin/activate
```

**3. Installera beroenden:**

```bash
pip install -r requirements.txt
```

**4. Kontrollera att `psutil` är installerat:**

```bash
pip show psutil
```

Du ska se information om psutil-paketet.

**5. Kör CPU-exemplet:**

```bash
python cpu_usage.py
```

Du får då ut aktuell CPU-användning i procent.

**Felsökning:**

- Får du fel om att `psutil` saknas? Kontrollera att du är i rätt miljö och att installationen lyckades.
- Får du "Permission denied"? Kontrollera att du har rättigheter till mappen.
- Vill du installera om alla paket? Ta bort `.venv`-mappen och börja om från steg 2.

**Vill du ändra koden?**

Redigera `cpu_usage.py` för att visa mer information eller göra fler mätningar.

---

> "A true hero isn't measured by the size of his strength, but by the strength of his heart"
> 
> – Zeus
