# HH Sisäinen JavaScript-koulutus

##Alkuun pääseminen

##### BOOTTAA XUBUNTU-DVD:LTÄ (14.04 LTS)
> ei tarvitse asentaa - valitse, että kokeilet vaan Xubuntua

##### KÄYNNISTÄ TERMINAL EMULATOR
`ctrl`+`alt`+`t`

#####NÄPPÄIMISTÖASETTELU SUOMEKSI
```sh
setxkbmap fi
```
#####LIITÄ MYY TIEDOSTOJÄRJESTELMÄÄSI
```sh
sudo mkdir /mnt/myy
sudo mount.cifs //myy/<omatunnus> -o username=<omatunnus>
```
> syötä salasana myylle

#####LISÄÄ PAKETTIENHALLINTAJÄRJESTELMÄÄN ULKOINEN LÄHDE
```sh
sudo add-apt-repository ppa:webupd8team/sublime-text-2
```

#####PÄIVITÄ PAKETTIENHALLINTAJÄRJESTELMÄN TIETOKANTA
```sh
sudo apt-get update
```

#####ASENNA TEKSTIEDITORI
```sh
sudo apt-get install sublime-text
```
> voit käynnistää Sublime Text Editorin komentoriviltä komennolla `subl`

#####ASENNA CHROMIUM-SELAIN
```sh
sudo apt-get install chromium-browser
```
> voit käynnistää selaimen komennolla `chromium-browser`

#####ASENNA VERSIONHALLINTATYÖKALU
```sh
sudo apt-get install git
```
> Kyllä, voit käyttää lisää levytilaa: Y

#####KOPIOI KURSSIMATERIAALIT VERSIONHALLINNASTA
```sh
#Siirry työskentelemään myylle
cd /mnt/myy
#luo versionhallintaa varten oma hakemisto
mkdir git
#mene äsken luodun kansion sisään
cd git
#kloonaa koulutusmateriaali verkosta uuteen alihakemistoon
git clone https://github.com/jleikko/JS-koulutus.git
```

##### REKISTERÖIDY GITHUBIIN
```sh
chromium-browser http://github.com &
```
> ellet ole jo rekisteröitynyt

#####ASENNA KONEELLESI NODE.JS JAVASCRIPT-YMPÄRISTÖ
```sh
#asenna node.js runtime
sudo apt-get install nodejs
#asenna node package manager
sudo apt-get install npm
#asenna vielä tuki ohjelmille, jotka ovat riippuvaisia noden binääristä
sudo apt-get install nodejs-legacy
```
> Kyllä, voit käyttää lisää levytilaa: Y

#####ASENNA RAKENNUSTYÖKALU YEOMAN
```sh
#suorita globaali asennus Yeoman-työkalulle node package managerin avulla
sudo npm install -g yo
#asenna webbisovelluspohjageneraattori
npm install -g generator-webapp
#asenna angular-webbisovelluspohjageneraattori
npm install -g generator-angular
```
> Kyllä, voit käyttää lisää levytilaa: Y

