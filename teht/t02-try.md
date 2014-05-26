## TEHTÄVÄ 2 - OHJELMOINTIA JAVASCRIPTILLÄ

#####Kopioi tehtäväpohja itsellesi

```sh
cp ~/git/JS-koulutus/teht/t02-try-material/index.html ~/git/JS-harjoitukseni/t02-try/
```

#####Tutustu sovelluksen toiminnallisuuteen
```sh
chromium-browser ~/git/JS-harjoitukseni/t02-try/index.html &> /dev/null &
```


#####Avaa HTML-tiedosto editoriin muokattavaksi

```sh
subl ~/git/JS-harjoitukseni/t02-try/index.html &> /dev/null &
```

#####Tee tiedostoon lisäyksiä

1. Lisää nappi "Punaiseksi" ja tee se toimivaksi.
2. Lisää nappi "Vihreäksi" ja tee se toimivaksi.
3. Tee napeista sellaiset, että jos painat yhtä nappia kaksi kertaa peräkkäin, laatikko muuttu valkoiseksi.
4. Tee toinen laatikko nappien alapuolelle.
5. Lisää napit "Kapeaksi" (-> 50px) ja "Leveäksi" (-> 200px) toisen laatikon alapuolelle. Tee näistäkin napeista toggle-tyyppiset.
6. Lisää sivulle kolmas laatikko, jonka sisällä oleva piiloitettu "Lorem ipsum"-teksti tulee näkyviin, kun käyttäjä vie hiiren kolmannen laatikon päälle ja katoaa taas, kun käyttäjä vie hiiron pois.

#####Tallenna tehtävä GitHubiin

```sh
cd ~/git/JS-harjoitukseni
git add .
git commit -m 'Toka tehtävä tehty'
git push
```
