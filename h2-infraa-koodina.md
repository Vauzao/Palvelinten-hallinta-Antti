# H2 Infraa koodina

x)
## Karvinen 2014: Hello Salt Infra-as-Code: 

- Teimme tähän liittyvän tehtävän tunnilla
- Yksinkertainen hello world print

## Salt contributors: Salt overview:

- YAML on oletus renderöijä
- Renderöijä kääntää yaml data rakenteen python data rakenteeksi

## Salt contributors: The top file:

- Top file tiedostossa on hallittujen koneiden konfiguraatioiden ja ryhmien kartoitus.

## Hei infra koodi
a)

- Tämä tehtävä tehtiin tunnilla
- Tein kansion hellolle mkdir komennolla
- Vaihdoin samaan hakemistoon itseni
- editoin tiedoston nanolla ja laitoin sinne tarvittavan sisällön, että hello world toimi
- Kokeilin että se toimii komennolla: salt-call --local state.apply hello

## Topfile
b)

- Käytin apuna : Salt contributors: The top file sivua.
- Varmistin oikean tiedosto sijainnin
- Tein top tiedoston /srv/salt/top.sls
- Laitoin esimerkin nano tiedostoon - core ja - edit
- Sitten muokkasin - core ja - edit tiedostojen sisältöä haluamakseni
- lopuksi testasin että ne toimivat komennolla: sudo salt-call --local state.apply

## Viisikko
c) 

- Loin viisikolle omat tiedostot mkdir komennolla
- esimerkiksi hellopkg.init.sls
- tein kaikkiin nano tiedostoihin esimerkit, jotka löysin 
- sitten testasin että toimiiko ne komennolla: sudo salt-call --local state.apply
- Vastaus: 6 onnistui 1 epäonnistui
- Epäonnistuneessa oli pieni kirjoitusvirhe

## Kaksi eri tilafunktiota
d)

- esimerkkinä pkg ja service
- esimerkissä asensin htop: Install_htop
- ja varmistin että ssh palvelu toimii: ensure_sshd_running
- Aluksi toinen näistä epäonnistui syntaksi virheen takia, mutta löysin ongelman nopeasti.
- Testasin ajaa komennolla: sudo salt-call --local state.apply multistate
- Testasin, että tiedosto on idempotentti


Lähteet
https://terokarvinen.com/2024/hello-salt-infra-as-code/
https://docs.saltproject.io/salt/user-guide/en/latest/topics/overview.html#rules-of-yaml
https://docs.saltproject.io/en/latest/ref/states/providers.html




