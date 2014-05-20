##WORKFLOW

#####ASENNA RAKENNUSTYÖKALU YEOMAN (EI TOIMI VÄLTTÄMÄTTÄ KUNNOLLA)
```sh
#suorita globaali asennus Yeoman-työkalulle node package managerin avulla
cd /mnt
sudo npm install -g yo
#asenna webbisovelluspohjageneraattori
sudo npm install -g generator-webapp
```
#####LUO WEBBIPROJEKTIPOHJA
```sh
#siirry oikeaan hakemistoon
cd /mnt/myy/git/t3
#generoi sivustollesi runko
yo webapp
#asenna riippuvuus boweriin
bower install underscore
#buildaa asennusvalmis sovellus
grunt
```

#####AVAA TIEDOSTOT MUOKATTAVAKSI
```sh
avaa sublime-text editori oikeassa hakemistossa
subl &> /dev/null &
```

#####TESTAA WEBBIPROJEKTIA
```sh
grunt serve
```
> Jos muokkaat tiedostoja sublimella, muutosten pitäisi näkyä heti tallennuksen jälkeen selaimessa
