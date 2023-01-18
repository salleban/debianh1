# debianh1
Installing Debian 11 in virtual machine

## Oracle VM VirtualBox Manager

Lähdetään luomaan uutta käyttöjärjestelmää VirtualBoxin avulla. Aloitettiin valitsemalla vasemmasta yläkulmasta Machine -> New...
Tästä edettiin valitsemalla alhaalta painike Expert Mode. Tämän avulla lähdetään syöttämään ennakkotieto asennusta varten. 
Edetään järjestyksessä ja varmistetaan ennen kolmatta kohtaa, että varmasti on Debianin .iso tiedosto ladattu koneen tiedostoihin ja haetaan ISO Image kenttään oikea tiedosto. Seuraavalla välilehdellä Unattended Install syötetään käyttäjänimi sekä vahvat salasanat kirjautumista varten. 
Hardware välilehdellä syötetään Base Memory kohtaan 4000MB. Processors kohta pidetään sellaisenaan 1CPU. 
Hard Disk kohtaan Create a Virtual Hard Disk Now annetaan default vaihtoehto kohteelle, mutta syötetään 20 GB -> 60GB, jotta saadaan enemmän tilaa toiminnoille. 
Hard Disk File Type and Variant asetetaan VDI (VirtualBox Disk Image). 

Tämän jälkeen tarkistetaan, että tiedosto polut on samat ylimmässä ja alimmassa välilehdessä, jolloin asennus alkaa toimimaan. Paina lopuksi Finish. 

## Debian käynnistys

Ennen Debianin käynnistystä pitää mennä Settings -> Storage ja valita tämän jälkeen Storage Devices -> Controller: IDE ja valitaan Debian-live-11.6.0... ja tämän jälkeen lisätään Attributes kohtaan Optical Drive ja painetaan vetovalikon päässä olevasta cd painikkeesta oikea optinen asema. Sitten painetaan OK ja käynnistetään Debian. 

## Debian aloitus

Käynnistyttyään valitaan Debian GNU/Linux Live (kernel 5.10.0-20-amd64) (paina enter). Tässä menee hetki ennenkuin pääsee jatkamaan. Valittuani Debian GNU/Linux Live (kernel 5.10.0-20-amd64) ilmestyy ruutuun Debian logo, jonka ympärillä pyörii hiljakseen valkoinen kehä. Tämän jälkeen ruutu menee mustaksi, ja hetken kuluttua ilmestyy tekstiä missä ilmenee "Error, failed to send host log message". Ruutu pysyi mustana n. 15 min ajan ennen kuin login screen tuli esille. Kuitenkin kirjautuessa tulee valitus, että salasana on väärä, joten tämän pitemmälle en ole kyennyt vielä pääsemään. Seuraavaksi koneet kiinni ja jatketaan seuraavana päivänä, mielessäni uusi kikka, mutta ladataan ensin akut, jotta jaksaaa keskittyä. 

## Debian jatkoa

Seuraava päivä ja kokeiltiin erilaista lähestymistapaa. Poistettiin VirtualBox versio 7.0.6 ja asennettiin vanhempi versio 6.1.42 tilalle. 
Heti huomaan, että valikot ovat hieman erilaiset ja näyttävät enemmän tehtävään liittyvän ohjeistuksen mukaisilta. Etenen ohjeiden mukaisesti ja lopulta valitsen Optical Disk Selectorista oikean debian-live-11.6.0-amd64-xfce+nonfree.iso tiedoston ja valitsen Choose ja tämän jälkeen Start. 

Debian käynnistyy ja valitsen menu valikosta Debian GNU/Linux Live (kernel 5.10.0-20-amd64). Nyt jännistys kävi korkealla, sillä näin pitkälle en ollut ennen päässyt. Tällä kertaa tulee noin 1-2 minuutin odottelun jälkeen oikea näkymä, eli työpöytä. Nyt päästään etenemään tehtävässä. 

## Debian käyttöä

Alku hehkuttelun jäljiltä palasin ohjeistuksien pariin ja lähdin testailemaan toimivuuksia. Vasemman yläkulman Application painikkeesta hain Web Browser painikkeen, painelin täydellä teholla Googleen ja googlasin ilman mitään sitä miettimättä ohjeistuksen mukaisesti Tero Karvinen ja löysin tieni terokarvinen.com kotisivuille, kaikki näyttää siis toimivan mainiosti. 

## Debian Installation

Seuraavaksi valitaan työpöydän vasemmasta alakulmasta Install Debian painike ja aloitetaan asennus ja edetään seuraavasti:
    - Kieli, American English -> Next
    - Location, Suomi (Valitse painamalla Suomea kartasta) -> Next 
    - Valitse vasemmasta valikosta Finnish ja jätä oikeanpuoli kohtaan Default. Keyboard Model kohdassa pitäisi näkyä Generic 105-key PC (intl.) -> Next 
    - Seuraavaksi valitaan Erase disk, jätetään alempaa Encrypt system valitsematta ja alimpana oleva valikko Boot loader location valitaan Master Boot Record... -> Next
    - Sitten täytetään käyttäjätietoja. Ensimmäiseen kohtaan oma nimi, toinen on kirjautumisnimi, tähän valitaan pienellä kirjoitettuna max 8 kirjainta/numeroa oleva yhdistelmä. Seuraavaan kohtaan älä laita omaa nimeäsi, yritä nimetä kone mahdollisimman anonyymisti. 
    - Viimeisempänä valitse vahva salasana itsellesi, jokin sellainen, mitä et ole ennen käyttänyt.
    - Älä laita rastia Log in automatically without asking for the password. -> Next
    
Summary kohdassa on yhteenveto. Jos kaikki näyttää hyvältä, paina Install. Tämä saattaa viedä noin 10min aikaa. Nyt on aika tankata vesipullot!

Asentelun jälkeen ruutuun pamahtaa teksti All done. Valitaan rasti ruutuun Restart now(pitäisi olla automaattisesti valittuna) ja tämän jälkeen painetaan Done. 

## Loppu selvennys

Näin on saatu valmiiksi Debianin asennus VirtualBoxiin. Alun takkuilun jälkeen asennus oli äärimmäisen helppo. Mikäli ongelmia tulee, kannattaa hetkeksi pysähtyä ja miettiä vaihtoehtoisia ratkaisuja ongelmiin, näin kävi minun tapauksessani.


