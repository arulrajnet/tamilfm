TamilFM
========

Online playlist of all tamil radios. View the live player at <a href="http://tamilfm.arulraj.net/">http://tamilfm.arulraj.net/</a>


###Setup

NodeJS on ubuntu

```
sudo apt-get install node
sudo npm install -g grunt-cli
sudo ln -s "$(which nodejs)" /usr/bin/node
```

To build

```
grunt build
```


### To change to playlist

Update either the **src/js/app/playlist.js** or .xml file. If you are going to use the XML file, you will need to set the "useJsonPlaylist" variable to false in the **src/js/app/app.js** file and then run grunt build.

### All thanks goes to

* JPlayer - <a href="https://github.com/happyworm/jPlayer">https://github.com/happyworm/jPlayer</a>
* Circle Player - <a href="https://github.com/maboa/circleplayer">https://github.com/maboa/circleplayer</a>
* Responsive JPlayer - <a href="https://github.com/BeyondHyper/responsive-jPlayer">https://github.com/BeyondHyper/responsive-jPlayer</a>

Hosted on github pages. Fork of <a href="https://github.com/BeyondHyper/responsive-jPlayer">reponsive jPlayer</a>
