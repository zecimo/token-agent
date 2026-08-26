# Token Agent

Aplicație desktop (Windows / macOS) care face legătura între zecimo și tokenul
criptografic SafeNet (sau orice token PKCS#11 compatibil) de pe calculatorul tău.

Serverul nu are acces direct la token: îi trimite agentului comenzile de semnare,
iar agentul le execută local, cu certificatul care rămâne tot timpul pe token.

## Instalare

Descarcă instalatorul pentru sistemul tău din [ultimul release](https://github.com/zecimo/token-agent/releases/latest):

| Sistem | Fișier |
|---|---|
| Windows (x64) | `TokenAgentSetup.exe` |
| macOS (Apple Silicon) | `TokenAgent-osx-arm64.dmg` |
| macOS (Intel) | `TokenAgent-osx-x64.dmg` |

După instalare, deschide agentul și conectează-l la workspace-ul tău cu codul de
împerechere din zecimo (Setări → Token Agent).

## Actualizări

Agentul verifică singur dacă există o versiune nouă și se actualizează în fundal.
Nu trebuie să reinstalezi nimic manual.

## Despre acest repo

Aici stau **doar** instalatorii și pachetele de actualizare. Codul sursă face parte
din monorepo-ul zecimo (folderul `TokenAgent/`) și este privat.
