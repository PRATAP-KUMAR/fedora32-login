# fedora32

_**This script assumes that the Installation of Fedora32 is a fresh install. If you tried to change the GDM background with someother scripts, you first need to reset those changes. Other scripts may have the option --reset.**_

_**Recovery from fatal errors: If you encounter any problems after running this script..
log on to any tty**_
````
sudo rm /usr/share/gnome-shell/gnome-shell-theme.gresource
sudo dnf reinstall gnome-shell
reboot
````

Required Package: glib2-devel
```
sudo dnf install glib2-devel
````

this script is to change the login screen background of Fedora32 only.

you can download the file `fedora32-login` via command line

    wget -qO - https://github.com/PRATAP-KUMAR/fedora32-login/archive/master.tar.gz | tar zx --strip-components=1 fedora32-login-master/fedora32-login

Once you downloaded the script `fedora32-login`. cd to the downloaded script file.

to set the background with Image  
`sudo ./fedora32-login /absolute/path/to/image`

to set the background with color  
`sudo ./fedora32-login \#aAbBcC` replace `#aAbBcC` with any vaid hex color code..

to reset everything that the script made..  
`sudo ./fedora32-login --reset`

![Black Color](https://i.imgur.com/RA00k0D.png)

![Background as Image](https://i.imgur.com/4IK7T9a.png)
