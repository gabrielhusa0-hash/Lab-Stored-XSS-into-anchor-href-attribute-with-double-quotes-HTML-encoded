# Stored XSS into anchor href attribute with double quotes HTML-encoded

## 📚 Studijní materiál
Tento repozitář slouží jako můj osobní studijní zápisník a přehled řešení laboratoří z platformy **PortSwigger Web Security Academy**. Dokumentuji zde postupy, zranitelnosti a způsob jejich exploitationu pro budoucí reference a rozvoj znalostí v oblasti kybernetické bezpečnosti.

---

## 🛠️ Postup řešení laboratoře

1. **První komentář:** Nejprve jsem napsal komentář s libovolným textem (např. "hello my friends"), vyplnil jméno, email a do políčka pro web (Website) jsem zadal `securityc0de`, odeslal jsem ho a vrátil se zpět.
2. **Druhý komentář:** Následně jsem napsal další komentář (např. "hi my friends"), změnil jméno autora, email nechal stejný.
3. **Vložení payloadu a dokončení:** Do políčka pro web (a případně všude kromě emailu) jsem napsal payload `javascript:alert(1)`, odeslal jsem to,  stránka byla laboratoř úspěšně vyřešena.