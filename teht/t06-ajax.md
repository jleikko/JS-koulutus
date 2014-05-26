## TEHTÄVÄ 6 - AJAX

##### Avaa esimerkkisovellus

```sh
#käynnistä palvelin (sulkeutuu komennolla ctrl-c)
cd ~/git/JS-koulutus/teht/t06-ajax-materiaali 
python -m SimpleHTTPServer
#käynnistä selain
chromium-browser http://localhost:8000/index.html &> /dev/null &
```

Tutki miten sovellus toimii ja miten se on rakennettu.
Katso siirtyvien json-olioiden sisältöä Chromiumilla:
Developer Tools->Network->henkilot.json->Response

##### Tee oma AJAX-tekniikkaa käyttävä säätietosovellus JQueryllä

Toteuta säätietosivu käyttäen taustalla palvelua http://openweathermap.org/API. Toteuta cross-domain json-haku jsonp-tekniikalla. Käytä tallennukseen omaa repositoryasi 'cd ~/git/JS-harjoitukseni/t06-ajax/'. Commitoi ja pushaa GitHubiin aktiivisesti.
