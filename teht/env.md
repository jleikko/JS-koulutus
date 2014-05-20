##KÄYTTÖJÄRJESTELMÄ KUNTOON

##### BOOTTAA XUBUNTU-DVD:LTÄ (14.04 LTS)
> ei tarvitse asentaa - valitse, että kokeilet vaan Xubuntua

##### AVAA SELAIN OHJESIVULLE
http://github.com/jleikko

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

#####ASENNA SSH FILESYSTEM
```sh
sudo apt-get install sshfs
```

##TYÖTILA KUNTOON

#####LIITÄ MYY TIEDOSTOJÄRJESTELMÄÄSI
```sh
sudo mkdir /mnt/myy
sudo chown xubuntu:xubuntu /mnt/myy
sshfs -o idmap=user kayttajatunnuksesi@myy.haaga-helia.fi:/homeh/kayttajatunnuksesi /mnt/myy
# VANHA: sudo mount.cifs //myy/<omatunnus> -o username=<omatunnus>
# VANHA: sudo mount -t cifs -o username=h00916,uid=xubuntu,gid=xubuntu //myy/h00916 /mnt/myy
```
> syötä salasana myylle

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

#####REKISTERÖIDY GITHUBIIN
```sh
#TODO: PRINTIT POIS
chromium-browser http://github.com &
```
> ellet ole jo rekisteröitynyt

#####LUO UUSI REPOSITORY GITHUBIIN TEHTÄVIÄSI VARTEN
Anna repositoryn nimeksi *JS-harjoitukseni*


#####LATAA REPOSTASI PAIKALLINEN KOPIO
```sh
git clone https://github.com/<githubin_kayttajatunnuksesi>/JS-harjoitukseni.git
```

#####LUO HARJOITUKSIA VARTEN ETUSIVU JA HAKEMISTORAKENNE
```sh
cd JS-harjoitukseni
echo '#JS-harkat\nJavaScript-koulutuksen harjoituksia' > README.md
mkdir t1
touch t1/.gitkeep
mkdir t2
touch t2/.gitkeep
mkdir t3
touch t3/.gitkeep
```

#####LISÄÄ LUOMASI TIEDOSTOT COMMITOITAVAKSI STAGING-TILAAN
```sh
git add -A
```

#####COMMITOI MUUTOKSET LOKAALISTI
```sh
git commit -m 'hakemistorakenne luotu'
```

#####LÄHETÄ MUUTOKSET PALVELIMELLE
```sh
git push origin master
```
