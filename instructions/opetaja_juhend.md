# Õpetaja juhend: Digiloovtöö haldamine GitHubis

See juhend on mõeldud õpetajale Digiloovtöö aine läbiviimiseks, kasutades projektihalduskeskkonnana GitHubi. GitHub asendab varasemat Taiga keskkonda, pakkudes ühes kohas nii koodihoidlat, dokumentatsiooni (Wiki) kui ka projektijuhtimise tööriistu (Projects).

## 1. Ettevalmistus ja seadistamine

Erinevalt Taigast, kus õpetaja loob tihti ise projektiruumid, on GitHubis soovitatav lasta õpilastel võtta vastutus ja luua oma tiimi töökeskkond ise.

### Soovituslik töökorraldus:

1.  **Konto:** Veendu, et sul on GitHubi konto.
2.  **Jälgimine:** Palu igal tiimil lisada sind oma projekti (_Repository_) liikmeks (_Collaborator_), et saaksid jälgida protsessi ja hinnata tulemusi.
3.  **Mallid (Soovituslik):** Kui soovid, et kõigil oleks ühtne kaustastruktuur (nt kaustad `/dokumentatsioon`, `/kood`, `/meedia`), võid luua ühe näidis-repositooriumi (_Template Repository_) ja paluda õpilastel alustada tööd sellest koopia tegemisega ("Use this template").

## 2. Digiloovtöö mõistete vastavus GitHubis

Et säilitada aine metoodika (scrum, sprindid), tuleb terminid üle kanda GitHubi loogikale:

| Digiloovtöö / Taiga mõiste    | GitHubi vaste                   | Selgitus                                             |
| :---------------------------- | :------------------------------ | :--------------------------------------------------- |
| **Projekt**                   | **Repository**                  | Kogu tiimi töö (failid, wiki, haldus) asub siin.     |
| **Tahvel (Kanban)**           | **GitHub Projects**             | Töölaud veergudega (Todo, In Progress, Done).        |
| **User Story (Kasutajalugu)** | **Issue**                       | Üks konkreetne ülesanne või funktsionaalsus.         |
| **Sprint**                    | **Iteration** või **Milestone** | Ajavahemik tööde grupeerimiseks (nt Sprint 1).       |
| **Task (Alamülesanne)**       | **Task List**                   | _Issue_ sees olev nimekiri (`- [ ] tegevus`).        |
| **Wiki**                      | **Wiki**                        | Dokumentatsiooni (persoonad, stsenaariumid) asukoht. |

## 3. Hindamine ja monitooring

GitHub pakub väga täpset statistikat, mis lihtsustab individuaalse panuse hindamist.

### A. Individuaalse panuse hindamine

Ava tiimi repositoorium ja vali sakk **Insights** -> **Contributors**.

- **Mida jälgida:** Graafik näitab, kes ja millal on koodi lisanud (Commits).
- _Märkus:_ Projektijuhtimise panust (ülesannete liigutamine, kommenteerimine) näeb **Pulse** vaates, mitte koodi statistikas.

### B. Protsessi hindamine (Projektitahvel)

Ava sakk **Projects**.

- Vaata, kas _Issue_'d liiguvad reaalajas või tehakse kõik viimasel hetkel.
- Klõpsates suvalisel _Issue_'l, näed selle ajalugu (kes alustas, kaua võttis aega).

### C. Dokumentatsiooni hindamine

Ava sakk **Wiki**.

- Paremal servas on nupp **Page History**, mis näitab täpselt, milline õpilane millist dokumentatsiooni osa täiendas.

## 4. Õpetaja tegevused semestri jooksul

1.  **Algus:** Taga, et õpilased on loonud _Repository_, aktiveerinud _Projects_ vaate ja lisanud sinna esimesed "Digiloovtöö" analüüsiga seotud ülesanded (persoonade loomine jne).
2.  **Sprintide lõpp:** Vaata üle projektitahvel. Kas "Done" veerus olevad asjad on reaalselt valmis (kontrolli _Acceptance Criteria_ täitmist)?
3.  **Tagasiside:** Jäta kommentaare otse _Issue_'de alla või koodi ridadele (_Code review_). See on õpilasele õpetlikum kui üldine tagasiside e-koolis.
