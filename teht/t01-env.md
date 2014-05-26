##KÄYTTÖJÄRJESTELMÄ KUNTOON

##### BOOTTAA XUBUNTU-DVD:LTÄ (14.04 LTS)
* Valitse kieleksi Suomi
* Ei tarvitse asentaa - valitse, että kokeilet vaan Xubuntua

##### AVAA SELAIN OHJESIVULLE
https://github.com/jleikko/JS-koulutus/blob/master/teht/t01-env.md
> Web-selain löytyy ruudun vasemmasta yläkulmasta.

##### KÄYNNISTÄ TERMINAALI
`ctrl`+`alt`+`T`
> Terminaaliin voi liittää leikepöydältä tekstiä komennolla `ctrl`+`shift`+`V`

#####LISÄÄ PAKETTIENHALLINTAJÄRJESTELMÄÄN ULKOINEN LÄHDE
```sh
sudo add-apt-repository ppa:webupd8team/sublime-text-2
```

#####PÄIVITÄ PAKETTIENHALLINTAJÄRJESTELMÄN TIETOKANTA
```sh
sudo apt-get update
```
##TYÖKALUT KUNTOON

#####ASENNA KOODARILLE SOVELTUVA TEKSTIEDITORI
```sh
sudo apt-get install sublime-text
```
> voit käynnistää Sublime Text Editorin komentoriviltä komennolla `subl`

#####ASENNA CHROMIUM-SELAIN
```sh
#asenna selain pakettienhallintajärjestelmän kautta
sudo apt-get install chromium-browser
#vaihda chromium oletusselaimeksi
xdg-settings set default-web-browser chromium.desktop
```
> voit käynnistää uuden selaimen komennolla `chromium-browser`. Mikäli haluat, ettei selainprosessi varaa komentoriviä lokitustaan varten, voit käynnistää selaimen komennolla `chromium-browser >& /dev/null &`

#####ASENNA VERSIONHALLINTATYÖKALU
```sh
#asenna git client pakettienhallintajärjestelmän kautta
sudo apt-get install git
#konfiguroi git clienttiin oma nimesi ja sähköpostiosoitteesi
git config --global user.name "<Oma Nimi>"
git config --global user.email "<oma_sahkoposti>"
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
> Luo git-hakemisto omaan kotihakemistoosi. Terminaali käynnistyy oletuksena omaan kotihakemistoosi, ja voit palata kotihakemistoosi aina komennolla `cd`

#####REKISTERÖIDY GITHUBIIN
https://github.com/join
> ellet ole jo rekisteröitynyt

#####LUO UUSI REPOSITORY GITHUBIIN TEHTÄVIÄSI VARTEN
Anna repositoryn nimeksi "JS-harjoitukseni"
> uusi repository voidaan luoda vihreästä napista rekisteröitymisen jälkeen

#####LATAA REPOSTASI PAIKALLINEN KOPIO
```sh
git clone https://github.com/<githubin_kayttajatunnuksesi>/JS-harjoitukseni.git
```

#####LUO HARJOITUKSIA VARTEN ETUSIVU JA HAKEMISTORAKENNE
```sh
cd JS-harjoitukseni
echo '#JavaScript-koulutuksen harjoitukset' > README.md
mkdir t02-try
touch t02-try/.gitkeep
mkdir t03-func
touch t03-func/.gitkeep
mkdir t04-obj
touch t04-obj/.gitkeep
mkdir t05-ajax
touch t05-ajax/.gitkeep
mkdir t06-node
touch t06-node/.gitkeep
mkdir t07-workflow
touch t07-workflow/.gitkeep
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
git push -u origin master
```
