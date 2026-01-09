# `.gitignore`

Selles peatükis räägime, kuidas kasutada `.gitignore` faili, et hoida repositoorium puhtana, jättes välja failid ja kaustad, mis ei paku versioonihalduses väärtust või failid, mis sisaldavad tundlikke andmeid.

![gitignore](gitignore.webp)

Pildi allikas: Dall-E by OpenAI

- [`.gitignore`](#gitignore)
  - [.gitignore Node.js kontekstis](#gitignore-nodejs-kontekstis)
    - [Selgitus eelnevast näitest](#selgitus-eelnevast-näitest)
    - [Mida panna `.gitignore`](#mida-panna-gitignore)
    - [Mida mitte panna `.gitignore`](#mida-mitte-panna-gitignore)
  - [Harjutused](#harjutused)

Lühidalt kirjeldades on `.gitignore` fail, mis sisaldab reegleid failide ja kaustade kohta, mida Git peaks ignoreerima, ehk mida ei tohiks versioonihaldusesse lisada, nagu näiteks erinevad salajased või keskkonnapõhised failid, ajutised failid, keskkonnapõhised failid ja kolmanda osapoole sõltuvused.

## .gitignore Node.js kontekstis

Siin on näide tüüpilisest `.gitignore` failist Node.js projektidele:

```plaintext
# Logid
logs/
*.log
npm-debug.log*

# Käitusaegsed andmed
pids/
*.pid
*.seed
*.log

# Teekide kaust jscoverage/JSCover poolt genereeritud instrumenteeritud teekide jaoks
lib-cov/

# Katvuse kaust, mida kasutavad tööriistad nagu istanbul
coverage/

# nyc testi katvus
.nyc_output/

# Sõltuvuste kaust
node_modules/

# IDE - Integreeritud Arenduskeskkonna seaded
.idea/
.vscode/

# Keskkonnamuutujad (dotenv failid)
.env
.env.test

# Mac failid
.DS_Store

# Vabatahtlik npm vahemälu kaust
.npm

# Vabatahtlik eslint vahemälu
.eslintcache

# Vabatahtlik REPL ajalugu
.node_repl_history
```

### Selgitus eelnevast näitest

- **Logid:** Tavaliselt jäetakse logifailid ja -kaustad ignoreerituks, kuna need sisaldavad sageli käitusaegseid andmeid, mida ei ole vaja versioonida.
- **Käitusaegsed andmed:** Samuti tuleks välja jätta kõik genereeritud PID või seemnefailid.
- **Testi katvuse andmed:** Kaustad nagu `lib-cov`, `coverage` ja `.nyc_output` sisaldavad testidega kaetuse andmeid ja tuleks välja jätta.
- **`node_modules/`:** See on Node.js projektide jaoks oluline kaust, mida ei ole vaja versioonihaldusesse kaasata. Kui paigaldada kolmanda osapoole pakette `npm`-i või `yarni` kaudu, salvestatakse need paketid sellesse kausta. See kaust tuleks välja jätta, sest:

- see võib olla suur, muutes kloonimise ja tõmbamise aeglaseks;
- sõltuvused saab installida keskkonnapõhiselt. See tagab, et kui teine arendaja või CI/CD (*Continuous Integration/Continuous Delivery*, Pidev Integreerimine/Pidev Tarnimine ) kloonib repositooriumi, paigaldatakse täpselt need versioonid, mis on määratud vastavalt `package-lock.json` või `yarn.lock` failides.
- **IDE seaded:** Kaustad nagu `.idea/` (JetBrainsi IDE-dele) ja `.vscode/` (Visual Studio Code'ile) sisaldavad kasutajaspetsiifilisi koodieditori seadeid. Neid tuleks ignoreerida, et vältida teise arendaja seadistuse ülekirjutamist.
- **Keskkonnamuutujad:** Failid nagu `.env` sisaldavad sageli tundlikke või keskkonnapõhiseid väärtusi. Neid tuleks ignoreerida, et vältida tundliku informatsiooni lekkimist ja võimaldada erinevatel arendajatel või keskkondadel säilitada oma spetsiifilisi konfiguratsioone.
- **Maci-spetsiifilised:** `.DS_Store` on Mac OS-i poolt genereeritud süsteemifail, mis ei ole rakenduse koodi jaoks vajalik.
- **Vahemälu failid:** `.npm` ja `.eslintcache` on vahemälu kaustad/failid, mida ei ole vaja versioonida.
- **REPL ajalugu:** `.node_repl_history` on ajaloo fail, kui kasutate Node REPL-i (käsurea keskkond).

### Mida panna `.gitignore`

- Genereeritud ja ajutised failid.
- Keskkonnapõhised failid.
- Kolmanda osapoole sõltuvused (nagu `node_modules/`).
- IDE ja redaktori konfiguratsioonifailid.
- Saladused ja konfiguratsioonifailid keskkonnapõhiste väärtustega.
- OS-spetsiifilised failid (nagu `.DS_Store`).

### Mida mitte panna `.gitignore`

- Projekti lähtekood ja failid, mis koodiga kaasnevad.
- Konfiguratsioonifailid, mis on vajalikud rakenduse käitamiseks ja jagatud kõigi projekti instantside vahel (välja arvatud saladused).
- Dokumentatsioon ja sellega seotud varad.
- Ehitus- ja juurutusskriptid.
  
Pidage meeles, et `.gitignore` faili eesmärk on hoida teie repositoorium puhtana, jättes välja failid ja kaustad, mis ei paku versioonihalduses väärtust. See aitab ka vältida tundliku andme või kasutajaspetsiifiliste seadete mittetahtlikult versioonihaldusesse lisamist.

## Harjutused

Proovi selgitada oma sõnadega, mis on `.gitignore` ja miks see on oluline.

Järgmisena proovi lõpetada järgmised ülesanded:

- Loo oma repositooriumis `.gitignore` fail.
- Lisa `draft.md` `.gitignore` faili.
- `commit`-i .gitignore` fail oma repositooriumisse.
- Loo uus fail nimega `draft.md` ja lisa sinna mõningane sisu.
- Kontrolli, kas `draft.md` on Git'i poolt ignoreeritud (proovi seda `commit`-ida).
