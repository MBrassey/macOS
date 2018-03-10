[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=KYEHRWKYCD3A2)
<h1>Desktop Configuration </h1>

This is my macOS High Sierra configuration. 

See: <a href="https://github.com/mattinclude/Bash/tree/master/braindumpToolkit">braindumpToolkit</a> ( Beta ) for converting pdf's for certdragon.

<h1>Features</h1>
<ul>
  <li>Responsive Angular JS.</li>
  <li>Exam Objectives, Practice Exams and Timed Exam Simulator.</li>
  <li>Randomized Questions and Answers.</li>
  <li>Review Correct Answers.</li>
  <li>Load Multiple Exams with Multiple Parts.</li>
  <li>Designed for Quickly Preparing for Real Exams.</li>
  <li>Place Files on your Webserver or use the Docker Capability.</li>
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

<h1>Pull from Docker index</h1>
<pre>
docker pull mattinclude/certdragon
</pre>

<h1>Build it yourself</h1>
<pre>
git clone https://github.com/mattinclude/certdragon.git
<br>
docker build --rm -t mattinclude/certdragon certdragon
<br>
docker run -d -h certdragon -p 80:80 -d -i mattinclude/certdragon
</pre>

<h1>Connect to certdragon web-interface (Windows)</h1>

Find certdragon's container IP address (Usually 192.168.99.100):
<pre>
docker-machine ls
</pre>
Or...
<pre>
docker-machine ip default
</pre>

Navigate to this IP address using your web browser or launch the container's web preview using Kitematic.

<h1>Connect to certdragon web-interface (Mac)</h1>

Open Web Browser:
<pre>
Navigate to localhost.
</pre>

<h1>How to Uninstall</h1>

Stop & Remove certdragon using the following <b>three</b> commands within the Docker Terminal:
<pre>
docker stop $(docker ps -a -q | grep -v mattinclude/certdragon) && docker rmi -f mattinclude/certdragon
</pre>
Stop / Remove ALL docker containers:
<pre>
docker stop $(docker ps -a -q) <br>
docker rm $(docker ps -a -q)
</pre>

<h1>Troubleshooting</h1>
Docker: dial tcp: lookup index.docker.io: no such host
<pre>
docker-machine ssh default <br>
sudo sed -i '1s/^/nameserver 8.8.8.8\n/' /etc/resolv.conf && exit
</pre>

<h1>Credits</h1>
<pre>
Music: Angela J. Brassey
Sounds: Freesound.org
braindumpToolkit: Matthew A. Brassey
AngularJS: Ken Tilly
System Platforms: ubuntu, apache2, Docker, certDragon
</pre>
