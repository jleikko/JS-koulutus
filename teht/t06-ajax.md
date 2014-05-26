## Ajax

##### Avaa esimerkkisovellus

```sh
#käynnistä palvelin (sulkeutuu komennolla ctrl-c)
cd ~/git/JS-koulutus/teht/t06-ajax-materiaali 
python -m SimpleHTTPServer
#käynnistä selain
chromium-browser http://localhost:8000/index.html &> /dev/null &
```

Tutki miten sovellus toimii ja miten se on rakennettu.

##### Tee JS-harjoitukseni-repon kansioon "t06-ajax" uusi sovellus. Commitoi ja pushaa aktiivisesti GitHubiin.

###### Tehtävänanto

Toteuta säätietosivu käyttäen taustalla palvelua http://openweathermap.org/API. Toteuta cross-domain json-haku jsonp-tekniikalla.
