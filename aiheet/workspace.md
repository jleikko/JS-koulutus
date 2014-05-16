##TYÖTILA KUNTOON

#####LIITÄ MYY TIEDOSTOJÄRJESTELMÄÄSI
```sh
sudo mkdir /mnt/myy
# VANHA: sudo mount.cifs //myy/<omatunnus> -o username=<omatunnus>
sudo mount -t cifs -o username=h00916,uid=xubuntu,gid=xubuntu //myy/h00916 /mnt/myy
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
chromium-browser http://github.com &
```
> ellet ole jo rekisteröitynyt

#####LUO UUSI REPOSITORY GITHUBIIN TEHTÄVIÄSI VARTEN
Anna repositoryn nimeksi *JS-harjoitukseni*


#####LATAA REPOSTASI PAIKALLINEN KOPIO
```sh
git clone https://github.com/<kayttajatunnuksesi>/JS-harjoitukseni.git
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
