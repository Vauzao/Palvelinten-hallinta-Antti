# H3 soitto kotiin

## x) Tiivistys
Karvinen 2021: Two Machine Virtual Network With Debian 11 Bullseye and Vagrant:
-	On hyvää harjoittelua tuhota virtual machine ja aloittaa alusta.
-	Vagrant auttaa kahden koneen yhdistämisessä
Karvinen 2018: Salt Quickstart – Salt Stack Master and Slave on Ubuntu Linux:
-	master$ ja slave$ promptit
Karvinen 2023: Salt Vagrant - automatically provision one master and two slaves:
-	Samoja asioita kuin aikaisemmin top sls ja infra as code on tuttuja
-	Aina kaksi välilyöntiä tekstissä
-	
## a) Vagrant asennus
- Latasin vargrantin latauslinkin kautta
- Tarkistin cmd kautta, että se on asennettuna: vargrant –version.
- Vagrantin versio numero oli 2.4.9
- 
## b) Linux Vagrant
- Tein hakemiston: mkdir vagrant-linux-testi ja siirryin hakemistoon cd komennolla
- Käytin komentoa vagrant init, mutta sain errorin siitä että vagrantia ei löytynyt.
- Ja  sitten  sudo apt install vagrant -y
- Tarkistin, että debianissa on nyt vagrant komennolla: vagrant –version ja vastaukseksi tuli: vagrant 2.3.8
- sitten  vagrant init debian/bookworm64. 

## c) Kahden tietokoneen verkko
- Menin linux testi hakemistoon
- Muokkasin siellä nano Vagrantfile tekstitiedostoa.
- Laitoin sinne valmiin scriptin sivulta: https://terokarvinen.com/2021/two-machine-virtual-network-with-debian-11-bullseye-and-vagrant/.
- Tämän jälkeen käytin komentoa: vagrant up.
- Koneet pystyivät pingata toisiaan komennolla: ping (iposoite)

## d) Salt minion 
- Mennään t001 sisään komennolla: vagrant ssh t001
- Sitten sudo apt install -y salt-master
- Ja sydo systemctl enablella salt master päälle
- Sama t002 koneelle
- Lisäsin nano tiedostoon masterin iposoitteen
- Ja sudo salt-key -A
- Lopuksi tein pingauksen testiksi

## e) Keskeneräinentehtävä
- Teen e tehtävän valmiiksi huomenna, kello on  5 yöllä, ja olen tehnyt tehtävää monta tuntia.
  Lähteet:
  
  https://terokarvinen.com/2021/two-machine-virtual-network-with-debian-11-bullseye-and-vagrant/
  https://terokarvinen.com/2018/salt-quickstart-salt-stack-master-and-slave-on-ubuntu-linux/?fromSearch=salt%20quickstart%20salt%20stack%20master%20and%20slave%20on%20ubuntu%
  https://terokarvinen.com/2023/salt-vagrant/#infra-as-code---your-wishes-as-a-text-file
  https://oispadotka.wordpress.com/2020/05/12/h6/
