##WORKFLOW

#####ASENNA RAKENNUSTYÖKALU YEOMAN (http://yeoman.io/)
```sh
#siirry oikeaan hakemistoon
cd ~/git/JS-harjoitukseni/t07-workflow
#suorita globaali asennus Yeoman-työkalulle node package managerin avulla
npm install -g yo
#asenna webbisovelluspohjageneraattori
npm install -g generator-webapp
```
#####LUO WEBBIPROJEKTIPOHJA
```sh
#generoi sivustollesi runko
yo webapp
```

#####AVAA TIEDOSTOT MUOKATTAVAKSI
```sh
#avaa editori
subl . &> /dev/null &
```

#####KÄYNNISTÄ PALVELIN
```sh
grunt serve
```

#####MUOKKAA TIEDOSTON INDEX.HTML SISÄLTÖÄ

1. Avaa tiedosto `app/index.html` sublimen editori-ikkunaan.
2. Lisää oma nimesi jumbotron-divin sisään
3. tallenna (`ctrl`+`S`).

> muutosten pitäisi näkyä heti tallennuksen jälkeen selaimessa
