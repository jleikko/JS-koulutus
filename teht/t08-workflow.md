##WORKFLOW

#####ASENNA RAKENNUSTYÖKALU YEOMAN (http://yeoman.io/)
```sh
#suorita globaali asennus Yeoman-työkalulle node package managerin avulla
cd
npm install -g yo
#asenna webbisovelluspohjageneraattori
npm install -g generator-webapp
```
#####LUO WEBBIPROJEKTIPOHJA
```sh
#siirry oikeaan hakemistoon
cd ~/git/JS-harjoitukseni/t07-workflow
#generoi sivustollesi runko
yo webapp
```

#####AVAA TIEDOSTOT MUOKATTAVAKSI
```sh
#avaa sublime-text editori oikeassa hakemistossa estäen konsolilokitus
subl . &> /dev/null &
```

#####TESTAA WEBBIPROJEKTIA
```sh
grunt serve
```
> Jos muokkaat tiedostoja sublimella, muutosten pitäisi näkyä heti tallennuksen jälkeen selaimessa
