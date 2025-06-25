# Oppimispolku DataCenterFromZero

0. Lähtötilanne – Sovellus on kasvanut yli olemassa olevien rajojen

Yrityksen X mobiilisovelluksella on:

    Nopeasti kasvanut käyttäjäkunta (kymmenistä tuhansista satoihin tuhansiin tai miljooniin)

    Verkkosivuston ja GitHubin kapasiteetti ja suorituskyky eivät enää riitä

    Käyttäjät valittavat hitautta, katkoksia ja skaalautumattomuutta

    Tarve hallita itse laitteistoa, suorituskykyä, tietoturvaa ja kustannuksia

➡️ Tästä syntyy päätös: Perustetaan oma datakeskus.

1. Strateginen päätöksenteko ja liiketoimintaperustelut
Päätöksentekijät:

    Johto, CTO, CFO, mahdollisesti hallitus

Tehtävät:

    Kustannusvertailu: jatketaanko pilvessä, ulkoistetaanko vai rakennetaanko oma

    TCO-analyysi: arvioidaan elinkaarikustannukset (rakentaminen, ylläpito, energiankulutus)

    Skaalautuvuus: tuleeko oma datakeskus todella tarjoamaan parempaa kontrollia ja suorituskykyä?

    Ympäristövaikutukset ja regulaatiot (esim. EU CSRD, energiatehokkuusdirektiivit)

➡️ Tuloksena: liiketoimintapäätös oman datakeskuksen perustamisesta.

2. Arkkitehtuurisuunnittelu ja sijainnin valinta
Suunnittelijat:

    IT-arkkitehdit, laitesuunnittelijat, energia-asiantuntijat

Tehtävät:

    Sijainnin valinta: sähkön hinta, viiveet, kaapelointi, veden saatavuus (jäähdytys), luonnonriskit

    Kapasiteettisuunnittelu:

        Kuinka monta rackia, kuinka paljon tehoa per rack (kW)

        Tarvitaanko GPU-klustereita, AI-infrastruktuuria?

    Sähkönsyöttö ja UPS-ratkaisut (varavoima, generaattorit)

    Jäähdytysärjestelmä: ilmajäähdytys, nestejäähdytys, waste heat -talteenotto

    Yhteydet: kuituverkot, reititys, BGP, CDN

➡️ Tuloksena: tekninen suunnitelma ja alustavat piirustukset

3. Rakennusprojekti ja laitehankinnat
Osallistujat:

    Kiinteistökehittäjät, sähkö- ja LVI-insinöörit, laitehankintatiimi

Tehtävät:

    Rakennetaan fyysinen tila tai valitaan modulaarinen esivalmistettu ratkaisu

    Hankitaan laitteisto:

        Palvelimet (blade, rack)

        Tallennusratkaisut (NAS, SAN, SSD-pohjaiset järjestelmät)

        Kytkimet, palomuurit, reitittimet

        Rackit, kaapelointi, jäähdytys

➡️ Tuloksena: valmis tila, laitteet toimitettuna


4. Asennus, konfigurointi ja testaus
Vastuut:

    DevOps, infra-asiantuntijat, tietoturva, QA-tiimi

Tehtävät:

    Verkon perustaminen ja suojaus

    Asennetaan käyttöjärjestelmät ja alustat (esim. Kubernetes-klusterit, Docker, virtualisointi)

    Suojaus ja valvonta (firewall, IDS/IPS, SIEM, auditointi)

    Stressitestit ja varmistus: sovelluskuormien ajaminen, failover-skenaariot

➡️ Tuloksena: toimiva perusinfrastruktuuri


5. Sovelluksen siirto ja tuotantoon vienti
Projektitiimi:

    Sovelluskehittäjät, tietokanta-asiantuntijat, DevOps

Tehtävät:

    Migroidaan käyttäjädata, backend-palvelut ja API:t

    Järjestetään nollakatkojen siirtymä tai vaiheistettu käyttöönotto

    Monitorointi, lokienkeruu ja skaalautuvuusratkaisut käyttöön

➡️ Tuloksena: sovellus toimii omassa datakeskuksessa, käyttäjien kokemus paranee


6. Operointi, ylläpito ja optimointi
Ylläpitäjät:

    Sysadminit, NOC-tiimi, energiatehokkuusvastaavat

Tehtävät:

    Päivittäinen operointi, huoltotyöt, laitevaihdot

    Energian- ja lämmönkulutuksen optimointi

    Tietoturvaprosessien jatkuva valvonta

    Auditoinnit ja raportointi (myös ympäristöraportit jos EU-direktiivit koskevat)

➡️ Tuloksena: skaalautuva, tehokas ja vastuullinen oma datakeskus


Green ICT -suunnittelu alusta asti

Jos yritys X haluaa toimia vastuullisesti:

    Valitaan uusiutuva energialähde

    Jäähdytysjärjestelmä mahdollistaa hukkalämmön hyödyntämisen

    Modulaarinen rakenne mahdollistaa skaalauksen ilman suurta rakentamista

    Materiaalit valitaan kierrätettäviksi


  
### Yhteenveto päätöksentekijän näkökulmasta

| Vaihe          | Päätöksentekijän vastuu                                                     |
|----------------|-----------------------------------------------------------------------------|
| Strategia      | Hyväksyy investoinnin liiketoimintaperustein                                |
| Arkkitehtuuri  | Varmistaa että ratkaisu tukee pitkän aikavälin kasvua                       |
| Rakentaminen   | Varmistaa aikataulu ja budjetti                                             |
| Käyttöönotto   | Tukee muutosjohtamista ja asiakaskokemusta                                  |
| Operointi      | Varmistaa, että investointi toimii – teknisesti ja liiketoiminnallisesti    |









