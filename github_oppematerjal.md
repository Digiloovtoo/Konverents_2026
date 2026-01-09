# GitHub ja GitHub Projects: algtaseme õppevahend

## Sissejuhatus

GitHub on veebipõhine platvorm, mis võimaldab arendajatel ja meeskondadel koostööd teha, koodi hallata ning projekte planeerida. See tutvustav materjal on mõeldud algajatele, kes soovivad mõista GitHubi põhifunktsioone ja kasutada GitHub Projects tööriista õppe- või arendusprojektide haldamiseks.

## Miks GitHub?

Git ja GitHub on tänapäeval väga laialdaselt kasutusel olev ja oluline tööriist tarkvaraarenduses ning ka muudes valdkondades, kus on vaja versioonihaldust ja koostööd. Peamised eelised on:

- Koostöö: kõik failid ja arutelud ühes kohas ja on näha kes mida ja millal muutis.
- Versioonihaldus: võimalik naasta eelmiste versioonide juurde.
- Läbipaistvus: ülesanded, arutelud, kood ja otsused on jälgitavad.

## Põhisõnavara (git ja GitHub)

- `repository` (repo): projekti "kaust" GitHubis, sisaldab faile ja ajalugu.
- `commit`: salvestuspunkt muudatusega (koos sõnumiga).
- `branch`: paralleelne arendusliin (nt main on põhiline).
- `merge`: haru liitmine teise haruga.
- `pull request` (PR): ettepanek muudatuse liitmiseks; sisaldab arutelu ja koodivaatamist.
- `fork`: repo koopia, mida saab iseseisvalt muuta.
- `clone`: repo koopia tõmbamine oma arvutisse.
- `push`: oma lokaalsete muudatuste GitHubi saatmine.
- `pull`/`fetch`: muudatuste tõmbamine GitHubist enda arvutisse.
- `issue`: ülesande või probleemi kirjeldus.
- `project`: planeerimistahvel, mis seob `issue`id.

## GitHubi põhi-struktuur

- Konto või organisatsioon sisaldab repositooriume.
- Repositoorium sisaldab faile, kaustu, commite, harusid ja `issue`id.
- Projects (uue põlvkonna) on eraldi vaated (tahvel/board), kuhu saab `issue`id linkida ning välju (omanik, tähtaeg) hallata.
- Lisakanalid: Wiki (püsidokumendid) ja Discussions (arutelud).

## Repo sisu, mida kohe märgata

- **README.md**: projekti avaleht ja juhised.
- **LICENSE**: litsents, mis määrab kasutusõiguse.
- **.gitignore**: failid/kaustad, mida versioonihaldus ei jälgi.
- Kaustastruktuur: kood, dokumentatsioon, andmed (väldi suuri binaare).

## Markdown kiirjuhend

Markdown on lihtne märgistuskeel, mida GitHub kasutab dokumentide vormindamiseks (nt README.md). Märgendikeel tähendab seda, et tekstile lisatakse lihtsad sümbolid, ehk märgendid, mille abil kirjeldatakse, mida see tekst parasjagu tähendab (pealkiri, loetelu, link vms). Nende märgendite põhjal otsustab GitHub või mõni muu tööriist, kuidas see tekst kasutajale kuvatakse (nt pealkirjad on suuremad ja paksus kirjas, lingid on klikitavad jne).

### Markdowni Põhielemendid:

- Pealkirjad: `#`, `##`, `###`
- Loendid: `-` või `1.`
- Koodiplokid: ` ` (mitmerealine) või `järjekordselt` (üksik rida)
- Lingid: `[tekst](url)`
- Tabeli alus: `| Veerg1 | Veerg2 |` + eraldusrida `| --- | --- |`
- Rõhud: `**rasvane**`, `_kaldkiri_`

## GitHub Projects (planeerimine)

GitHub Projects on tööriist, mis võimaldab hallata ülesandeid ja projekte visuaalselt. Uus Projects (v2) pakub paindlikkust ja integreerimist `issue`dega.

### Projects-i põhikomponendid:

- **Vaated**: Board (kanban), Table, Timeline.
- **Kaardid**: issues või draft items.
- **Väljad**: status (To do / In progress / Done), assignee, due date, priority.
- **Automaatika**: reeglid (nt staatuse muutmisel liigub kaart veergude vahel).
- **Õppetöös**: defineeri teemad issues’ena, jälgi edenemist boardil, seo kaardid konkreetsete õppijatega.

## Tüüpiline õppevoog (lihtne)

1. Loo repo (või kasuta olemasolevat).
2. Lisa README.md juhistega.
3. Loo Project board (nt Kanban) veergudega To do / In Progress / Done.
4. Loo issues iga ülesande/teema kohta.
5. Õppija: clone repo → tee muudatus → commit lokaalselt → push.
6. Õppejõud või meeskond vaatab muudatuse üle (näiteks branchide võrdlusega) ja liidab sobival ajal põhiharuga.
7. Liiguta issue/kaart boardil Done veergu.

## Rollid ja õigused (lihtsustatult)

- Owner: haldab seadeid ja õigusi.
- Maintainer/Collaborator: saab push’ida ja harusid merge’ida (vastavalt õigustele).
- Kontribuutor: teeb fork’i ja avab muudatusi läbi branchide (avatud repo puhul) või ettevalmistab paketid ülevaatuseks.
- Vaataja: loeb ja kommenteerib.

## Minimaalsed käsud algajale (CLI)

- git clone <url>: repo koopia.
- git status: vaata muutusi.
- git add <fail>: lisa muutus commit’i.
- git commit -m "Sõnum": salvesta punkt.
- git push: saada GitHubi.
- git pull: too värskendused GitHubist.
  Kui CLI tundub hirmutav, kasuta GitHub Desktopi või VS Code Source Control vaadet.

## Hea issue kirjutamise põhimõtted

- Issue: lühike pealkiri, kirjelda "mida" ja "miks", vajadusel ekraanipildid või näited.
- Lisa kontekst (kasutusjuht, ootused), et ülevaataja saaks aru eesmärgist.

## Tüüpilised vead, mida vältida

- Töötamine otse main-harus → tee eraldi branch.
- Suured commitid ilma sõnumita → tee väikseid, selgete sõnumitega.
- README ja juhendi puudumine → lisa alginfo ja käivitamisjuhis.
- Failide/kaustade segadus → hoia selge struktuur ja .gitignore.
