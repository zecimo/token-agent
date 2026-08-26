# Token Agent

Aplicație desktop care face legătura între zecimo și tokenul criptografic SafeNet
(sau orice token PKCS#11 compatibil) de pe calculatorul tău.

Serverul nu are acces direct la token: îi trimite agentului comenzile de semnare,
iar agentul le execută local, cu certificatul care rămâne tot timpul pe token.

## Instalare (Windows)

Descarcă `TokenAgent-win-Setup.exe` din [ultimul release](https://github.com/zecimo/token-agent/releases/latest) și rulează-l.

Instalatorul nu este semnat digital, așa că Windows va afișa un avertisment
SmartScreen la prima rulare — alege **Informații suplimentare → Executare oricum**.

După instalare, deschide agentul și conectează-l la spațiul tău de lucru cu codul
de împerechere din zecimo (Setări → Token Agent).

> macOS: nu există încă build publicat. Spune-ne dacă ai nevoie.

## Actualizări

Agentul verifică singur dacă există o versiune nouă și se actualizează în fundal.
Nu trebuie să reinstalezi nimic manual.

## Despre acest repo

Aici stau **doar** instalatorii și pachetele de actualizare. Codul sursă face parte
din monorepo-ul zecimo (folderul `TokenAgent/`) și este privat.
