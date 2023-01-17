# debianh1
Installing Debian 11 in virtual machine

## Oracle VM VirtualBox Manager

Lähdetään luomaan uutta käyttöjärjestelmää VirtualBoxin avulla. Aloitettiin valitsemalla vasemmasta yläkulmasta Machine -> New...
Tästä edettiin valitsemalla alhaalta painike Expert Mode. Tämän avulla lähdetään syöttämään ennakkotieto asennusta varten. 
Edetään järjestyksessä ja varmistetaan ennen kolmatta kohtaa, että varmasti on Debianin .iso tiedosto ladattu koneen tiedostoihin ja haetaan ISO Image kenttään oikea tiedosto. Seuraavalla välilehdellä Unattended Install syötetään käyttäjänimi sekä vahvat salasanat kirjautumista varten. 
Hardware välilehdellä syötetään Base Memory kohtaan 4000MB. Processors kohta jäteen sellaisenaan 1CPU. 
Hard Disk kohtaan Create a Virtual Hard Disk Now annetaan default vaihtoehto kohteelle, mutta syötetään 20 GB -> 60GB, jotta saadaan enemmän tilaa toiminnoille. 
Hard Disk File Type and Variant asetetaan VDI (VirtualBox Disk Image). 

Tämän jälkeen tarkistetaan, että tiedosto polut on samat ylimmässä ja alimmassa välilehdessä, jolloin asennus alkaa toimimaan. Paina lopuksi Finish. 

## Debian käynnistys

Ennen Debianin käynnistystä pitää mennä Settings -> Storage ja valita tämän jälkeen Storage Devices -> Controller: IDE ja valitaan Debian-live-11.6.0... ja tämän jälkeen lisätään Attributes kohtaan Optical Drive ja painetaan vetovalikon päässä olevasta cd painikkeesta oikea optinen asema. Sitten painetaan OK ja käynnistetään Debian. 

## Debian aloitus

Käynnistyttyään valitaan Debian GNU/Linux Live (kernel 5.10.0-20-amd64) (paina enter). Tässä menee hetki ennenkuin pääsee jatkamaan. Valittuani Debian GNU/Linux Live (kernel 5.10.0-20-amd64) ilmestyy ruutuun Debian logo, jonka ympärillä pyörii hiljakseen valkoinen kehä. Tämän jälkeen ruutu menee mustaksi, ja hetken kuluttua ilmestyy tekstiä missä ilmenee "Error, failed to send host...".

