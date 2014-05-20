##KÄYTTÖJÄRJESTELMÄ KUNTOON

##### BOOTTAA XUBUNTU-DVD:LTÄ (14.04 LTS)
> ei tarvitse asentaa - valitse, että kokeilet vaan Xubuntua

##### AVAA SELAIN OHJESIVULLE
https://github.com/jleikko/JS-koulutus/blob/master/teht/t01-env.md
> Selain (Firefox) löytyy ruudun vasemmasta yläkulmasta.
> Mikäli sinulla on jenkkinäppis, "kauttaviivan" saat tavuviivan paikalta ja tavuviivan saat plus-merkin paikalta.

##### KÄYNNISTÄ TERMINAALI
`ctrl`+`alt`+`t`

#####NÄPPÄIMISTÖASETTELU SUOMEKSI
```sh
setxkbmap fi
```

#####LISÄÄ PAKETTIENHALLINTAJÄRJESTELMÄÄN ULKOINEN LÄHDE
```sh
sudo add-apt-repository ppa:webupd8team/sublime-text-2
```

#####PÄIVITÄ PAKETTIENHALLINTAJÄRJESTELMÄN TIETOKANTA
```sh
sudo apt-get update
```
##TYÖKALUT KUNTOON

#####ASENNA TEKSTIEDITORI
```sh
sudo apt-get install sublime-text
```
> voit käynnistää Sublime Text Editorin komentoriviltä komennolla `subl`

#####ASENNA CHROMIUM-SELAIN
```sh
#asenna selain pakettienhallintajärjestelmän kautta
sudo apt-get install chromium-browser
#vaihda chromium oletusselaimeksi
#VANHA: sudo update-alternatives --config x-www-browser
xdg-settings set default-web-browser chromium.desktop
```
> voit käynnistää uuden selaimen komennolla `chromium-browser`

#####ASENNA VERSIONHALLINTATYÖKALU
```sh
sudo apt-get install git
git config --global user.name "<Oma Nimi>"
git config --global user.email <oma_sahkoposti>
```
> Kyllä, voit käyttää lisää levytilaa: Y

#####ASENNA SSH FILE SYSTEM
```sh
sudo apt-get install sshfs
```

##TYÖTILA KUNTOON

#####KOPIOI KURSSIMATERIAALIT VERSIONHALLINNASTA
```sh
#luo versionhallintaa varten oma hakemisto
mkdir git
#mene äsken luodun kansion sisään
cd git
#kloonaa koulutusmateriaali verkosta uuteen alihakemistoon
git clone https://github.com/jleikko/JS-koulutus.git
```

#####REKISTERÖIDY GITHUBIIN
```sh
#TODO: PRINTIT POIS
chromium-browser http://github.com >& /dev/null &
```
> ellet ole jo rekisteröitynyt

#####LUO UUSI REPOSITORY GITHUBIIN TEHTÄVIÄSI VARTEN
Anna repositoryn nimeksi 'JS-harjoitukseni'


#####LATAA REPOSTASI PAIKALLINEN KOPIO
```sh
git clone https://github.com/<githubin_kayttajatunnuksesi>/JS-harjoitukseni.git
```

#####LUO HARJOITUKSIA VARTEN ETUSIVU JA HAKEMISTORAKENNE
```sh
cd JS-harjoitukseni
echo '#JS-harkat\nJavaScript-koulutuksen harjoituksia' > README.md
mkdir t02-try
touch t02-try/.gitkeep
mkdir t06-ajax
touch t06-ajax/.gitkeep
mkdir t07-node
touch t07-node/.gitkeep
mkdir t08-workflow
touch t08-workflow/.gitkeep
```

#####LISÄÄ LUOMASI TIEDOSTOT COMMITOITAVAKSI STAGING-TILAAN
```sh
git add .
```

#####COMMITOI MUUTOKSET LOKAALISTI
```sh
git commit -m 'hakemistorakenne luotu'
```

#####LÄHETÄ MUUTOKSET PALVELIMELLE
```sh
git push origin master
```
