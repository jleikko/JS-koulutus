##WORKFLOW

#####ASENNA RAKENNUSTYÖKALU YEOMAN (http://yeoman.io/)
```sh
#suorita globaali asennus Yeoman-työkalulle node package managerin avulla
cd
sudo npm install -g yo
#asenna webbisovelluspohjageneraattori
sudo npm install -g generator-webapp
```
#####LUO WEBBIPROJEKTIPOHJA
```sh
#siirry oikeaan hakemistoon
cd ~/git/JS-harjoitukseni/t8
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
