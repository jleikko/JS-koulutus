# HH Sisäinen JavaScript-koulutus

##Alkuun pääseminen

####NÄPPÄIMISTÖASETTELU SUOMEKSI
```sh
setxkbmap fi
```
#####LIITÄ MYY JÄRJESTELMÄÄSI
```sh
sudo mkdir /mnt/myy
sudo mount.cifs //myy/<omatunnus> -o username=<omatunnus>
```
> syötä salasana myylle

###PÄIVITÄ PAKETTIENHALLINTAJÄRJESTELMÄN TIETOKANTA
```sh
sudo apt-get update
```

###ASENNA VERSIONHALLINTATYÖKALU
```sh
sudo apt-get install git
```
> Kyllä, voit käyttää lisää levytilaa: Y

###KOPIOI KURSSIMATERIAALIT VERSIONHALLINNASTA
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

###ASENNA NODEJS
```sh
sudo apt-get install nodejs
```
> Kyllä, voit käyttää lisää levytilaa: Y

###ASENNA NODEJS PACKAGE MANAGER
```
sudo apt-get install npm
```
> Kyllä, voit käyttää lisää levytilaa: Y

