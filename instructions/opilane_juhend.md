# Õpilase juhend: Projektihaldus ja koostöö GitHubis

Selles aines kasutame projektihalduskeskkonnana GitHubi. See juhend aitab sul seadistada oma tiimi töökeskkonna, planeerida sprinte ja dokumenteerida Digiloovtöö protsessi.

## 1. Konto ja projekti loomine

1.  **Konto:** Loo endale kasutaja aadressil [github.com](https://github.com/), kui sul seda veel pole.
2.  **Tiimi repositoorium:**
    - Üks tiimiliige logib sisse ja vajutab **+** (üleval paremal) -> **New repository**.
    - **Repository name:** Pane projektile nimi (nt `digiloovtoo-tiim-X`).
    - **Visibility:** Vali **Private** (kui ei ole kokku lepitud teisiti).
    - Lisa linnuke: **Add a README file**.
    - Vajuta **Create repository**.
3.  **Liikmete lisamine:**
    - Ava loodud repositooriumis **Settings** -> **Collaborators**.
    - Vajuta **Add people** ja lisa oma tiimikaaslased ning õpetaja (küsi õpetaja kasutajanime).

## 2. Projektitahvli (Kanban) seadistamine

Et hallata ülesandeid, tuleb luua projektitahvel.

1.  Ava oma repositooriumis sakk **Projects**.
2.  Vajuta **New project** (või "Link a project").
3.  Vali malliks **Board**.
4.  Luuakse tabel vaadetega: _Todo_, _In Progress_, _Done_.
5.  Anna projektile nimi ja salvesta.

## 3. Töö planeerimine ja User Stories

Digiloovtöös jagame suure eesmärgi väiksemateks kasutajalugudeks (_User Stories_). GitHubis on kasutajalugu = **Issue**.

### Kuidas luua ülesannet?

1.  Ava **Issues** sakk ja vajuta **New issue**.
2.  **Title:** Pane lühike ja tabav pealkiri (nt "Persoonade loomine" või "Kodulehe esilehe disain").
3.  **Description:** Kirjelda sisu. Kasuta formaati:
    - _KASUTAJA LUGU:_ "Külalisena soovin ma näha..."
    - _VASTUVÕTUKRITEERIUMID:_ (Millal on see valmis? nt "Pildid on üles laetud ja tekst on loetav.")
    - _TASK LIST:_ Saad teha nimekirja alamülesannetest:
      ```markdown
      - [ ] Otsi taustainfo
      - [ ] Kirjuta tekst
      ```
4.  **Assignees:** Määra paremalt menüüst, kes tiimist seda teeb.
5.  **Projects:** Seo see ülesanne parempoolses menüüs oma loodud projektiga (punkt 2).
6.  Vajuta **Submit new issue**.

## 4. Sprintide (Iteratsioonide) haldamine

Sprindi pikkus ja sisu lepitakse kokku tiimiga. GitHubis saad sprinte hallata kas **Milestones** või **Iterations** (Projects vaates) abil.

**Lihtne meetod (Projects vaates):**

1.  Ava oma **Projects** tahvel.
2.  Lisa uus väli (Field) nimega **Iteration**.
3.  Määra igale ülesandele (_Issue_), millisesse "Iteratsiooni" (Sprinti) see kuulub (nt Sprint 1: Nõuete analüüs).
4.  Nüüd saad tahvlit filtreerida sprindi järgi, et näha ainult käesoleva nädala tööd.

## 5. Dokumentatsioon (Wiki)

Digiloovtöö analüüsi osa (persoonad, stsenaariumid, kavandid) ei käi koodi hulka, vaid **Wikisse**.

1.  Ava repositooriumis sakk **Wiki** (kui seda pole, luba see _Settings_ alt).
2.  Vajuta **Create the first page**.
3.  Loo lehed vastavalt vajadusele, näiteks:
    - `Home` (Projekti üldinfo)
    - `Persoonad`
    - `Stsenaariumid`
    - `Tehniline dokumentatsioon`
4.  Wikis saad kasutada Markdowni tekstide vormindamiseks ja piltide lisamiseks.

## 6. Tööprotsess (Flow)

Igapäevane töö näeb välja selline:

1.  **Võta ülesanne:** Lohista projektitahvlil ülesanne veerust _Todo_ veergu _In Progress_.
2.  **Tee töö:** Kirjuta koodi, koosta dokumentatsiooni või disaini.
3.  **Raporteeri:** Kui kasutad koodi lisamiseks _Commits_, lisa kommentaari ülesande number (nt `Lisasin esilehe pildi, seotud #4`).
4.  **Lõpeta:** Kui töö on valmis ja vastab kriteeriumitele, lohista kaart veergu _Done_ ja sulge _Issue_.

---

**Edukat projektijuhtimist!**
