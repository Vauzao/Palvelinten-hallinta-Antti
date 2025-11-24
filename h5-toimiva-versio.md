# H5 Toimiva versio
## x) Lue ja tiivistä
Chacon and Straub 2014:
- 
## a) Online
- aluksi mkdir ja cd tehtävää varten
- ![Mkdir ja cd tehtävää varten](h51.jpg)
- Se aloitetaan komennolla: git init
- ![alt text](h52.jpg)
- Tässä välissä tehdään tekstitiedosto tehtävää varten ja lisätään sinne tekstiä
- sitten Lisätään gnu gpl 3 lisenssi:
- ![alt text](h53.jpg)
- Tiedoston lisäys git add ja commit:
- ![alt text](h54.jpg)
- Tässä välissä sähköposti ja käyttäjänimi lisäys komennoilla: git config --global user.email ja git config --global user.name
- - Sitten tein githubiin uuden repon tehtävälle
- Kopioin sieltä: git remote add origin"", git branch -M main ja git push -u origin main
- Ja hain tokenin jotta pystyin syöttämään sen debianiin
- ![alt text](h55.jpg)
- Tässä näkyy lopputulos kaikki git toimii
- ![alt text](h56.jpg)
  
## b) Dolly
- kloonasin gitin
- ![alt text](h57.jpg)
- Muokkasin tekstiedostoa
- ![alt text](h58.jpg)
- Lisäsin ne gittiin ja committasin
- ![alt text](h59.jpg)
- Tarkistin logista muutoksen
- ![alt text](h510.jpg)
- push palvelimelle
- ![alt text](h511.jpg)
- Muutokset githubissa
- ![alt text](h512.jpg)

## c) Doh!
- Muokkasin aluksi tekstitiedostoon turhaa tekstiä
- ![alt text](h5c1.jpg)
- Tarkistin statuksesta että oli "modified"
- ![alt text](h5c2.jpg)
- Ja tuhosin muutokset 
- ![alt text](h5c3.jpg)
- statuksesta tarkistus
- ![alt text](h5c4.jpg)

## d) Tukki
- Tarkistin lokin, siinä näkyy esim. commitit ja author 
- ![alt text](h5d1.jpg)
- Käytin lisäksi vielä: git log --patch, lokin yksityiskohtaiseen tarkastukseen
- ![alt text](h5d2.jpg)
- ja tarkastelin vielä lisää...
- ![alt text](h5d3.jpg)
