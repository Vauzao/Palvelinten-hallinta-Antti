# Pkg file service

## x) Lue ja tiivistä
- Artikkelissa oli selkeät SSH staten tekemiseen.
- Package-file-servicen avulla voi hallita suuria määriä daemoneita. 
## a) 
![alt text](debian1.jpg)
- Tajusin, että jostain syystä sshd ei ole asennettuna joten asensin sen.
-   ![alt text](debian2.jpg)
-    ![alt text](debian3.jpg)
- ![alt text](debian4.jpg)
- Sitten: sudoedit /etc/ssh/sshd_config ja lisäsin ylimääräisen portin, mutta jätin 22 portin vagrantia varten.
- ![alt text](debian5.jpg)
- ![alt text](debian6.jpg)
## SALT
- ![alt text](debian7.jpg)
- ![alt text](debian8.jpg)
## Saltille oman koneen asetukset
- ![alt text](debian9.jpg)
- ![alt text](debian10.jpg)
## Saltin ajo
- ![alt text](debian11.jpg)
- ![alt text](debian12.jpg)
## Korjaa itsensä
- ![alt text](debian13.jpg)
- ![alt text](debian14.jpg)
- ![alt text](debian15.jpg)
  ## Palautan tämän nyt ja jatkan B,C,D ja E tehtäviä omalla ajalla myöhemmin

