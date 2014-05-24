##NODE.JS


#####A-KOHTA: ASENNA KONEELLESI NODE.JS JAVASCRIPT-YMPÄRISTÖ
```sh
#asenna node.js runtime
sudo apt-get install nodejs
#asenna node package manager
sudo apt-get install npm
#asenna vielä nodejs:ään tuki ohjelmille, jotka ovat riippuvaisia noden binääristä
sudo apt-get install nodejs-legacy
#korjaa pari asetusta, jotta npm-komentoon ei tarvita pääkäyttäjää
npm config set prefix ~/npm
echo "\n\nexport PATH=$HOME/npm/bin:$PATH" >> ~/.bashrc
source ~/.bashrc
```
####B-KOHTA: TEE PALVELIN NODEJS:N WEBBISIVUJEN MUKAISESTI
