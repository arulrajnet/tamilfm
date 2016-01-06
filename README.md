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
npm install
grunt build
```

### To change to playlist

Update either the **src/js/app/playlist.js** or .xml file. If you are going to use the XML file, you will need to set the "useJsonPlaylist" variable to false in the **src/js/app/app.js** file and then run grunt build.


### Desktop App Ubuntu

If you have firefox in your machine

```
[Desktop Entry]
Version=1.0
Terminal=false
Type=Application
Name=Tamil Radio
GenericName=Online Radio
Comment=Online Radio / FM for tamil songs
Exec=firefox -width 640 -height 600 -chrome http://tamilfm.arulraj.net
Icon=/usr/share/icons/tamilradio.png
StartupNotify=true
Categories=Player;
Name[en_IN]=Tamil Radio
X-Desktop-File-Install-Version=0.22
```

If you have chromium in your machine. Chnage the Exec to

```
Exec=/usr/bin/chromium-browser --profile-directory=Default --app=http://tamilfm.arulraj.net
```

Create `/usr/share/applications/tamilradio.desktop` with above content and make that file as executable for all. Copy this <a href="http://tamilfm.arulraj.net/favicon-48x48.png">image</a> to /usr/share/icons/tamilradio.png and make readable for all.

### All thanks goes to

* JPlayer - <a href="https://github.com/happyworm/jPlayer">https://github.com/happyworm/jPlayer</a>
* Circle Player - <a href="https://github.com/maboa/circleplayer">https://github.com/maboa/circleplayer</a>
* Responsive JPlayer - <a href="https://github.com/BeyondHyper/responsive-jPlayer">https://github.com/BeyondHyper/responsive-jPlayer</a>
* Icons pack by - <a href="https://icons8.com">Icons8</a>

Hosted on github pages. Fork of <a href="https://github.com/BeyondHyper/responsive-jPlayer">reponsive jPlayer</a>
