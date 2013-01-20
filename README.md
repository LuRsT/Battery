# Battery ( for linux )

![image](http://i.imgur.com/mEEPD.png)

Battery is a little perl script that displays the battery status on your __tmux__ sessions or the __terminal__.

[Original repo](https://github.com/Goles/Battery) ( for MAC OS )

### Features

* Changes color to reflect battery status (Green, Yellow, Red)
* Displays battery percentage
* Graph bar changes it's values between 0 and 100%

### Requirements

Perl, which is installed in almost every linux distro by default, and acpi, may or may not be installed.

### Install

git clone this to your ~/bin folder or any ${PATH} where you can execute the script simply by calling it by name, or simply copy the ```battery``` file to your ${PATH}.

### Usage (Terminal)

* Run Battery (From the terminal)

    ``` battery ```

###### You should see something like this:

![image](http://i.imgur.com/SLSBg.png)

### Usage (tmux)

* Add the following line to your `~/.tmux.conf` file

    ``` set -g status-right "#(perl ${HOME}/bin/battery tmux)"```

* reload the tmux config by running `tmux source-file ~/.tmux.conf`.

###### You should now see something like this at the bottom right corner:

![image](http://i.imgur.com/Eaajb.png)
