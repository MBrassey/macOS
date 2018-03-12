[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=KYEHRWKYCD3A2)

<h1>Desktop Configuration</h1>

My macOS (High Sierra) desktop 

![macOS](/img/macOS.gif)


Software used:

        Xcode
        iTerm2
        Homebrew
        zsh + oh-my-zsh
        vim
        Zephyros
        okeanos
        gtop
        tty-clock
        cava (cli visualiser) + mosh (ssh)
        appleseed

This script is generally a good preparation step: <a href="https://github.com/mzdr/macOS"> When I do a clean macOS installation.</a>

<h1>Window Manager</h1>
I have a pseudo tiling window manager configured using <a href="https://github.com/sdegutis/zephyros">Zephyros</a> & <a href="https://github.com/stayradiated/okeanos">Okeanos</a> together. This is a video demonstration from <a href="https://github.com/stayradiated">stayradiated</a>, the creator of Okeanos: 
<br><br>
<a href="http://www.youtube.com/watch?feature=player_embedded&v=10Zwc6r5sLs
" target="_blank"><img src="http://img.youtube.com/vi/10Zwc6r5sLs/0.jpg" 
alt="Okeanos" width="240" height="180" border="10" /></a>

<h1>Terminal</h1>
I've configured iTerm2 in a few ways to suit my liking. Simply import my <a href="https://github.com/mattinclude/appleseed/tree/master/backup">iTerm2 profile json</a> or set up a few things manually. I imported the <a href="https://github.com/mattinclude/appleseed/tree/master/backup">Hybrid</a> color preset. Under window settings, my <strong>Transparency=19%</strong>, <strong>Style=No Title Bar</strong> and I'm using <strong>no Blurring</strong>. I'm using the <a href="https://github.com/powerline/fonts">powerline patched</a> <a href="https://github.com/mattinclude/appleseed/tree/master/backup">Hack font</a> | A typeface designed for source code. I prefer the <strong>zsh</strong>, and have provided my custom theme <a href="https://github.com/mattinclude/appleseed/tree/master/backup">trident.zsh-theme</a>. 
<br><br>

        PROMPT="%{$fg_bold[blue]%}───╼%{$reset_color%} "
        RPROMPT="%{$fg[cyan]%}ψ %M %{$fg[green]%}%~%{$reset_color%}"


![macOS](/img/trident_zsh.png)

<h1>appleseed</h1>
<a href="https://github.com/mattinclude/appleseed"> appleseed v1.0.0</a> Is a command line widget (CLW), I designed for macOS and iTerm2. It's a flexible platform for process automation and eye candy. It utilizes `imgcat` to view image files with the help of shell integration. For best results, launch in a tall by thin proportioned shell.

![appleseed](/img/appleseed.png)

<h1>Misc.</h1>
I recommend the <a href="https://github.com/mattinclude/appleseed/tree/master/backup">Hybrid</a> color theme for vim. In the macOS General settings, I have the Graphite Appearance, and am using the Dark bar and Dock. The command line visualizer I am utilizing is <a href="https://github.com/karlstav/cava">cava</a>. You can also use <a href="https://github.com/dpayne/cli-visualizer">cli-visualizer</a>. I run the sofware over a mosh (persistant ssh) session to a Linux VM or instance.   
