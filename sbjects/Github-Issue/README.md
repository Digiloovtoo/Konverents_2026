# Github Issue

Selles peatükis käsitleme _Github Issue_'de kasutamist ja kirjutamist.

![Issue](Issue.webp)

Pildi allikas: Dall-E by OpenAI

- [Github Issue](#github-issue)
  - [Õpiväljundid](#õpiväljundid)
  - [Mis on _Github Issue_?](#mis-on-github-issue)
  - [Miks kasutada _Github Issue_'sid?](#miks-kasutada-github-issuesid)
  - [_Issuede_ kirjutamise head tavad](#issuede-kirjutamise-head-tavad)
  - [Näide hästi struktureeritud _issuest_](#näide-hästi-struktureeritud-issuest)
  - [Näide mitte nii hästi kirjutatud _issuest_](#näide-mitte-nii-hästi-kirjutatud-issuest)
  - [Harjutused](#harjutused)

Kõik projektid vajavad süsteemi, mis aitaks töökulgu organiseerida ja sellel silma peal hoida. Selleks on palju erinevaid tööriistu, **GitHub Issues** on kõigest üks paljudest turul olemasolevatest.

## Õpiväljundid

Peale selle peatüki läbimist oskad:

- kirjeldada, mis on _Github Issue_ ja kuidas seda kasutada;
- luua _Github Issue_'d ja määrata neile _assignee_'d;
- kommenteerida ja sulgeda _Github Issue_'t;

## Mis on _Github Issue_?

Githubi kontekstis on _issue_ omadus, mis võimaldab kasutajatel jälgida konkreetse hoidla ülesandeid, vigu ja funktsioonitaotlusi. See on hea võimalus saada projekti olukorrast kiire ülevaade ja oma töövoogu vastavalt sellele planeerida ja prioritiseerida. *Issue*d on ka üks viis, kuidas projekti liikmed saavad suhelda hoidlas oleva projekti teemal ja jälgida selle edenemist. _Issuede_ võimalus tuleb kaasa iga loodud repositooriumiga ja lisaks suhtlusele moodustavad _issue_'d ka osa projekti dokumentatsioonist.

_Issue_ avab tavaliselt kasutaja ja selle saab määrata ühele või mitmele teisele kasutajale, kes selle probleemi kallal võiks töötada. _Issue_ võib sisaldada **pealkirja**, **kirjeldust**, **silte** ja muid metaandmeid, nagu **prioriteet** või selle parandamise eest vastutav **isik**.

Githubis on võimalik kasutada eelloodud malle levinumate _issuede_ avamiseks, nt _bug report_'id ja _feature request_'id. Malle saab ka ise luua, vastavalt oma projekti vajadustele.

## Miks kasutada _Github Issue_'sid?

GitHubi *issue*t saab kasutada erinevatel eesmärkidel, näiteks:

- Tööülesannete jaotamine
- Tähtaegade seadmine
- Vigade jälgimine tarkvaraprojektides
- Funktsiooni/omaduse taotluste ja täiustuste jälgimine
- Töö üle arutamine ja koordineerimine arendajate meeskonna vahel
- Konkreetsele hoidlale või projektile toe taotlemine või pakkumine

*Issue*t saab otsida ja filtreerida erinevate kriteeriumide alusel, nagu _Issue_ **number**, **pealkiri**, **autor**, **silt** ja **olek**. Neid saab ka **kommenteerida** ja **värskendada**, et kajastada jälgitava töö oleku **muutusi**. _Issuede_ otsingu kasutamine on soojalt soovitatav, et (nt suuremate projektide korral) vältida _issue_-duplikaate ehk sama või sarnase sisuga _issue_'de loomist. Teistel sarnastel tööriistadel on automaatne duplikaatide tuvastussüsteem tavaliselt olemas, Github Issues seda võimalust kahjuks ei paku. Küll aga on Githubis võimalus kasutajal endal _issue_ duplikaatidest teada anda ja sarnased probleemid kokku grupeerida. Selleks tuleb kasutada kommenteerimisel või vastamisel `duplicate of #*issue* nr`, `duplicate pull request` või `duplicate *issue*` märksõnu.

## _Issuede_ kirjutamise head tavad

- Hoia pealkirjad lühikesed ja konkreetsed
- Sisus kirjelda tausta (_context_), esita probleem või idee, paku välja lahendus või järgmine samm
- Kasuta _labeleid_, aga mitte liiga palju korraga
- Selguse huvides kasuta _markdown_ keelt vormistamiseks (listid, rõhuasetused, pildid, lingid jms)
- Kaasa teisi inimesi – _@mentions_ ja _assigned to_
- Enne _issue_ esitamist veendu, et sama/sarnast probleemi pole juba püstitatud – kasuta otsinguvõimalust!
- Tee vahet _issuel_ ja _discussionil_ – lahtisemateks aruteludeks on parem variant GitHub Discussions
- Lahendatud _issued_ sulge, et segadust vältida

## Näide hästi struktureeritud _issuest_

![hea tava näide](https://wiredcraft.com/images/posts/how_we_write_our_github_issues_2.png)

Konkreetne pealkiri, tausta kirjeldus, inimeste kaasamine ja järgmine samm välja pakutud.

## Näide mitte nii hästi kirjutatud _issuest_

![halb näide](https://wiredcraft.com/images/posts/how_we_write_our_github_issues_1.png)

Liiga pikk pealkiri, liiga üldine sisu.

## Harjutused

Selleks, et praktiseerida selles teemas õpitut, tehke järgmist:

- Loo mõne oma repositooriumisse `Issue`, lisa sinna pealkiri, kirjeldus ja mõned sildid
- Lisa `Issue`le `assignee`
- Lisa endale suunatud `Issue`le kommentaar
- Sulge enda loodud `Issue`, kui sellele on antud mõni kommentaar
