[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=KYEHRWKYCD3A2)
<h1>Desktop Configuration </h1>

This is my macOS High Sierra configuration. 

This script is a good preparation step: <a href="https://github.com/mzdr/macOS">When I do a clean macOS installation.</a>

<h1>Suggested Software:</h1>
<ul>
  <li>macOS High Sierra</li>
  <li>Xcode</li>
  <li>iTerm2</li>
  <li>Homebrew</li>
  <li>zsh</li>
  <li>vim</li>
  <li>Zephyros</li>
  <li>okeanos</li>
  <li>gtop</li>
  <li>tty-clock</li>
</ul>
<img src="https://raw.githubusercontent.com/mattinclude/certdragon/master/cD/images/certDragon-github.png">

<h1>How to use</h1>
Run from the docker index. Or you can place the files contained in the "cD" directory on your webserver's root directory. Edit the app/js/config.js file to change the root directory path.

<h1>Run from Docker index</h1>
You can pull, install & start the certdragon container using this command within the Docker Terminal:
<pre>
docker run -h certdragon -p 80:80 -d -i mattinclude/certdragon
</pre>
Run certdragon with logging:
<pre>
docker run -h certdragon -p 80:80 -t -i mattinclude/certdragon
</pre>
