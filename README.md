# HH Sisäinen JavaScript-koulutus

##Alkuun pääseminen

##### BOOTTAA XUBUNTU-DVD:LTÄ (14.04 LTS)
> Ei tarvitse asentaa, valitse, että kokeilet vaan Xubuntua

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

#####PÄIVITÄ PAKETTIENHALLINTAJÄRJESTELMÄN TIETOKANTA
```sh
sudo apt-get update
```

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

#####ASENNA NODEJS JA NODE PACKAGE MANAGER
```sh
sudo apt-get install nodejs
sudo apt-get install npm
#tuki ohjelmille, jotka ovat riippuvaisia noden binääristä
sudo apt-get install nodejs-legacy
```
> Kyllä, voit käyttää lisää levytilaa: Y

#####ASENNA NODEJS PACKAGE MANAGER
```

```
> Kyllä, voit käyttää lisää levytilaa: Y

