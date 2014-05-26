##NODE.JS


####A-KOHTA: ASENNA KONEELLESI NODE.JS JAVASCRIPT-YMPÄRISTÖ
```sh
#asenna node.js runtime
sudo apt-get install nodejs
#asenna node package manager
sudo apt-get install npm
#asenna vielä nodejs:ään tuki ohjelmille, jotka ovat riippuvaisia noden binääristä
sudo apt-get install nodejs-legacy
#korjaa pari asetusta, jotta npm-komentoon ei tarvita pääkäyttäjää
npm config set prefix ~/npm
echo -e "\n\nexport PATH=\$HOME/npm/bin:\$PATH" >> ~/.bashrc
source ~/.bashrc
```
####B-KOHTA: TEE PALVELIN NODEJS:N WEBBISIVUJEN MUKAISESTI

##### Luo tiedosto miniserver.js ja avaa se muokattavaksi
```sh
cd ~/git/JS-harjoitukseni/t07-node
subl miniserver.js &> /dev/null &
```

#####Tallenna tiedostoon seuraavanlainen koodi
```js
var http = require('http');
http.createServer(function (req, res) {
  res.writeHead(200, {'Content-Type': 'text/plain'});
  res.end('Hello World\n');
}).listen(1337, '127.0.0.1');
console.log('Server running at http://127.0.0.1:1337/');
```

#####Käynnistä palvelin
```sh
node miniserver.js
```

#####Kutsu pavelinta selaimella
```sh
chromium-browser http://127.0.0.1:1337
```
