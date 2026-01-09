# Markdown

Selles teemas õpime tundma Markdowni, mis on üks populaarsemaid teksti vormindamise keeli maailmas. Uurime selle funktsioone, õpime seda kasutama ja avastame, kuidas seda saab kasutada tarkvaraprojektide dokumentatsioonis, blogimises ja muudes eesmärkides.

![Markup](Markup-Language.webp)

Pildi allikas: Dall-E by OpenAI

- [Markdown](#markdown)
  - [Õpiväljundid](#õpiväljundid)
  - [Mis on Markdown?](#mis-on-markdown)
  - [Mis on märgendikeel?](#mis-on-märgendikeel)
  - [Markdowni eelised](#markdowni-eelised)
  - [Markdowni puudused](#markdowni-puudused)
  - [Millal kasutada Markdowni](#millal-kasutada-markdowni)
  - [Põhilised Markdowni süntaksid](#põhilised-markdowni-süntaksid)
    - [Pealkirjad](#pealkirjad)
    - [Rõhutamine](#rõhutamine)
    - [Loendid](#loendid)
      - [Märgistamata](#märgistamata)
      - [Nummerdatud](#nummerdatud)
    - [Lingid](#lingid)
    - [Pildid:](#pildid)
    - [Tsitaadid](#tsitaadid)
    - [Ridade kood](#ridade-kood)
    - [Koodiblokid](#koodiblokid)
    - [Horisontaaljoon](#horisontaaljoon)
    - [Tabelid](#tabelid)
    - [Ülesannete loendid](#ülesannete-loendid)
  - [Harjutused](#harjutused)

## Õpiväljundid

Pärast selle teema läbimist oskad:

- kirjeldada, mis on Markdown ja miks see on kasulik;
- kirjeldada Markdowni plusse ja miinuseid;
- kasutada Markdowni teksti vormindamiseks;
- kasutada Markdowni dokumentatsioonis, blogimises ja muudel eesmärkidel.
- kasutada Markdowni Githubis.

## Mis on Markdown?

Markdown on kerge märgendikeel, millel on lihtne tekstivormingu süntaks. See loodi John Gruber-i poolt 2004. aastal. Markdowni peamine eesmärk oli muuta inimestel teksti kirjutamine ja vormindamine lihtsaks viisil, mis on vabalt loetav ja mida saab konverteerida HTML-iks (või teisteks väljundvorminguteks).

## Mis on märgendikeel?

Märgendikeel on keel, mida kasutatakse teksti vormindamiseks või struktureerimiseks, lisades märgendeid või märke. Märgendid on tavaliselt mingid sümbolid või sümbolite kombinatsioonid, mis on lisatud teksti, et määratleda, millist vormingut või struktuuri mingi tekst peaks omama. Märgendikeeli kasutatakse laialdaselt dokumentatsioonis, veebilehtede loomisel, blogimises ja paljudes muudes kontekstides.

Levinumad märgendikeeled on näiteks:

- HTML
- XML
- LaTeX
- Markdown
- jmt

## Markdowni eelised

- **Lihtsus:** Markdowni on lihtne õppida ja kasutada. Selle süntaks on intuitiivne, mis tähendab, et ka mittetehnilised inimesed saavad selles formaadis kirjutamisega hõlpsasti alustada.
- **Loetavus:** Markdowni dokumendid koosnevad tavalisest tekstist, seega need on loetavad isegi ilma teisele formaadile konverteerimata.
- **_Kaasaskantavus_:** Kuna need on tavalised tekstifailid, on Markdowni dokumendid OS-agnostilised ja neid saab avada mis tahes tekstiredaktoriga.
- **Paindlik väljund:** Markdowni saab konverteerida mitmesugusteks formaatideks, sealhulgas HTML-iks, PDF-iks ja isegi MS Word'i või LaTeX formaati.
- **Levinud kasutamine:** Markdown-i toetavad paljud platvormid, nagu GitHub, Reddit, Stack Exchange ja isegi sõnumirakendused nagu Slack ja Discord. Samuit on Markdown populaarne valik dokumentatsiooni ja blogimise jaoks.
- **Versioonikontrolli sõbralik:** Kuna tegemist on tavalise tekstiga, töötab Markdown sujuvalt versioonikontrollisüsteemidega nagu Git.
- **Pole vaja spetsialiseeritud tarkvara:** Markdowni saab kirjutada mis tahes tekstiredaktoris. Lisaks on olemas spetsialiseeritud Markdowni redaktorid, mis pakuvad täiendavaid funktsioone, nagu eelvaade ja kiire konverteerimine.

## Markdowni puudused

- **Piiratud stiilimine:** Kuigi Markdown saab hõlpsasti hakkama põhilise vormindusega, ei sobi see dokumentide koostamiseks, mis nõuavad keerukaid stiile või paigutusi.
- **Ebajärjekindlused:** On mitmeid Markdowni variatsioone ja mitte kõik tööriistad ei toeta igat funktsiooni. Näiteks GitHubi Markdowni töötlus võib olla veidi erinev teistest platvormidest.
- **Pole ideaalne suurte dokumentide jaoks:** Kuigi Markdowni saab kindlasti kasutada suuremate dokumentide jaoks, ei pruugi see olla nii hallatav või struktureeritud kui teised selleks otstarbeks loodud vormingud.
- **Ei ole sisseehitatud eelvaadet:** Kui ei kasutata spetsialiseeritud Markdowni redaktorit, ei ole võimalik vormindatud väljundit eelvaadata ilma seda konverteerimata. Samas on võimalik osadele redaktoritele paigaldada pistikprogramme, mis võimaldavad eelvaadet, nagu näiteks VS Code koos Markdown All in One pistikprogrammiga.

## Millal kasutada Markdowni

- **Dokumentatsioon:** Paljud avatud lähtekoodiga projektid kasutavad oma README-failide ja dokumentatsiooni jaoks Markdowni, kuna see on lihtne ja GitHub toetab seda juba vaikimisi.
- **Blogimine:** Paljud blogiplatvormid ja staatiliste saitide generaatorid toetavad Markdowni, kuna see on loetav ja kasutajasõbralik.
- **Märkmete tegemine:** Markdown sobib suurepäraselt struktureeritud märkmete tegemiseks. On mitmeid märkmete tegemise rakendusi, mis toetavad Markdowni vormindust.
- **Online arutelud:** Platvormid nagu Reddit ja Stack Exchange kasutavad teksti vormindamisel kommentaarides ja postitustes Markdowni.
- **Raamatute kirjutamine:** Mõned autorid kasutavad Markdowni raamatute, eriti tehniliste raamatute kirjutamiseks, kuna see on lihtne ja võimaldab konvertimist erinevatesse formaatidesse.
- **Esitlused:** Tööriistad nagu Reveal.js või Marp võimaldavad Markdowni kasutades luua isegi esitlusi.
- **Õppematerjalid:** Markdown sobib suurepäraselt õppematerjalide, nagu õpetused, spikrid ja muu loomiseks. Seda formaati on lihtne kirjutada ja lugeda ning seda saab konverteerida mitmesugusteks formaatideks. Kui allikmaterjalis midagi muutub, peate vaid uuendama Markdowni faili ja uuesti genereerima väljundi.

Kokkuvõttes on Markdown suurepärane valik projektidele, mis nõuavad põhilist vormindust ilma keerukamate märgistuskeelte lisakoormata. Selle lihtsus ja loetavus on Markdowni peamised tugevused, kuid keerukamate paigutuste või ulatusliku stiilimise jaoks võivad sobida paremini teised formaadid.

## Põhilised Markdowni süntaksid

Siin on kiire viide põhilistele Markdowni süntaksitele:

### Pealkirjad

```markdown
# H1

## H2

### H3

#### H4

##### H5

###### H6
```

### Rõhutamine

```markdown
_italic_ või _italic_
**bold** või **bold**
**_italic ja bold_** või _**italic ja bold**_
~~läbikriipsutus~~
```

### Loendid

#### Märgistamata

```markdown
- Ese 1
- Ese 2
  - Alamese 2.1
  - Alamese 2.2
```

või

```markdown
- Ese 1
- Ese 2
  - Alamese 2.1
  - Alamese 2.2
```

#### Nummerdatud

```markdown
1. Esimene ese
2. Teine ese
   1. Alamese 2.1
   2. Alamese 2.2
```

> Github võib mõningal määral näidata Markdown-i erinevalt, näiteks eelpool toodud loendit näidatakse nii:

1. Esimene ese
2. Teine ese
   1. Alamese 2.1
   2. Alamese 2.2

### Lingid

```markdown
[Google](https://www.google.com)
```

### Pildid:

```markdown
![Alt tekst](url_pildile)
```

### Tsitaadid

```markdown
> See on tsitaat.
```

### Ridade kood

```markdown
Siin on `rida koodi`.
```

### Koodiblokid

Kasutades kolme tagurpidikoma:

<pre>
```
function example() {
  console.log("näide");
}
```
</pre>

Või süntaksiga esiletõstmisega:

<pre>
```javascript
function example() {
  console.log("näide");
}
```
</pre>

### Horisontaaljoon

```markdown
---
```

või

```markdown
---
```

### Tabelid

```markdown
| Päis 1 | Päis 2 |
| ------ | ------ |
| Lahtr1 | Lahtr2 |
| Lahtr3 | Lahtr4 |
```

### Ülesannete loendid

```markdown
- [x] Ülesanne 1 (tehtud)
- [ ] Ülesanne 2 (tegemata)
```

Pidage meeles, et erinevad platvormid või Markdowni maitseained võivad omada lisafunktsioone või väikseid erinevusi, kuid ülalolev katab põhilised ja üldiselt kasutatavad süntaksid.

Lugege lisaks [Markdowni juhendist](https://www.markdownguide.org/).

## Harjutused

- Looge oma hoidlasse `README.md` fail ja kirjutage sinna lühike tutvustus enda kohta, kasutades Markdowni süntaksit.
- Veenduge, et kasutate vähemalt 3 erinevat Markdowni süntaksit (nt pealkirjad, loendid, lingid, pildid jne).
- `commit`-ige ja tõugake oma muudatused oma hoidlasse.
- Kontrollige oma hoidlat GitHubis ja veenduge, et teie `README.md` fail kuvatakse korrektselt.
