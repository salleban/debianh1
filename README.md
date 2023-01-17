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

Debian käynnistyy ja tässä saattaa kestää tovi. 
