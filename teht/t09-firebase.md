## TEHTÄVÄ 9 - FIREBASE

###A) Käy Firebasen tutoriaali läpi

https://www.firebase.com/tutorial/#gettingstarted

###B) Tee oma sovellus, joka käyttää Firebasea

####Rekisteröidy Firebaseen

https://www.firebase.com/signup/

####Rakenna oma sovellus

#####Siirry oikeaan hakemistoon työskentelemään

```sh
cd ~/git/JS-harjoitukseni/t09-firebase
```

#####Luo webbiprojektipohja

```sh
yo webapp
```

#####Hae bowerin avulla lokaalit kopiot firebase-kirjastoista

```sh
bower install firebase
```

#####Lisää tiedostoon app/index.html viittaus kirjastoon
```js
<script src="../bower_components/firebase/firebase.js"></script>
```

#####Rakenna chat-sovellus, joka käyttää omaa firebase-kantaasi

Kirjoita JavaScript-koodisi tiedoston `scripts/main.js` sisään. Muista commitoida ja pushata GitHubiin aktiivisesti.
