# H! Viisikko 
## x) Tiivistys

Karvinen 2025: Install Salt on Debian 13 Trixie
- Lisätään hakemisto apt varten, jotta salt voidaan asentaa
- Ladataan salt
- Täytyy olla 100% luotto ohjelmistoon, joka ladataan

Karvinen 2023: Run Salt Command Locally
- Salt komentoja voi ajaa paikallisesti salt minionilla
- Sillä voi hallita isompia järjestelmä kokonaisuuksia

Karvinen 2018: Salt Quickstart – Salt Stack Master and Slave on Ubuntu Linux
- Saltilla voi hallita tuhansia tietokoneita, ja ne voivat olla missä vaan
- Slaven täytyy tietää missä master on
- Slavella on oma id ja sen voi nimetä

Karvinen 2006: Raportin kirjoittaminen
- Lähteisiin viittaaminen on tärkeää raporteissa
- Helppolukuisuus on tärkeää ja tekstin täsmällisyys

## a) Debianin asennus

-Asensin debianin ISO tiedoston

## b) Saltin asennus

- Latasin wgetin komennoilla sudo apt-get update ja sudo apt_get install wget.
- Tein hakemiston saltrepo/ komennolla mkdir saltrepo/ ja siirryin sinne komennolla cd saltrepo/
- Latasin tiedostot Saltin virallisten ohjeiden mukaan. 
- Tarkastelin mitä tiedostot sisältää. 
- Ensimmäinen tiedosto on julkinen avain, jonka avulla voin olla varma, että lataus on luotettava
- Toinen tiedosto on lähdelista, joka kertoo mitä ladataan
- Sitten kopioin avain ja lähdelistan oikeisiin hakemistoihin käyttäen cp komentoa
- lopuksi ladataan salt-minion ja salt-master
- Testasin, että Salt toimii oikein. 

## c) Viisi tärkeintä tilafunktiota

- pkg: Tällä voi hallita kaikkia ohjelmia 
- file: Luo tiedostoja ja niitä voi myös muokata haluamaksi
- service: Palveluiden hallintaa esim. voi käynnistää ohjelmia tai restartata
- user: Tämän avulla hallitaan käyttäjiä esim. Voi luoda käyttäjän.
- cmd: Suorittaa komentoja 
- Kaikki nämä vaikuttavat todella tärkeiltä, jotta salttia voi käyttää tehokkaasti 

## d) Esimerkki idempotenssista 

 - Jos pkg.installed tree ensimmäisellä kerralla salt tarkistaa onko tree asennettuna, jos ei ole se lataa sen.
 - Uudelleen sama tehtäessä se tarkistaa saman mutta state kertoo, että se on jo asennettuna, eikä muutoksia tarvitse tehdä
 - Komento antaa eri tuloksen riippuen, siitä onko se jo esim. asennettu/poistettu
Lähteet:
Karvinen 2025: Install Salt on Debian 13 Trixie: https://terokarvinen.com/install-salt-on-debian-13-trixie/
Karvinen 2023: Run Salt Command Locally: https://terokarvinen.com/2021/salt-run-command-locally/
Karvinen 2018: Salt Quickstart – Salt Stack Master and Slave on Ubuntu Linux: https://terokarvinen.com/2018/03/28/salt-quickstart-salt-stack-master-and-slave-on-ubuntu-linux/
Karvinen 2006: Raportin kirjoittaminen: https://terokarvinen.com/2006/06/04/raportin-kirjoittaminen-4/
