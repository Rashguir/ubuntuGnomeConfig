# Ubuntu Gnome installation

	sudo apt update
	sudo apt upgrade -y

## Graphical improvments

	cd Downloads
	wget https://dl.opendesktop.org/api/files/download/id/1488740853/ocs-url_3.0.0-0ubuntu1_amd64.deb
	sudo dpkg -i ocs-url_3.0.0-0ubuntu1_amd64.deb
	sudo apt --fix-broken install -y
	sudo dpkg -i ocs-url_3.0.0-0ubuntu1_amd64.deb

Then go to https://www.gnome-look.org/p/1167049/
and click on "Install" on the line OSX-Arc-Darker-v1.4.1.tar.gz or any newer version
select ocs-url by default on the prompt window and install.
Then go to https://www.gnome-look.org/p/1171688/
and install both "Shell" lines (i prefer dark).

	sudo add-apt-repository -y ppa:papirus/papirus
	sudo apt update
	sudo apt install -y papirus-icon-theme

Go to : https://extensions.gnome.org/
Install the browser plugin.
Install extensions:

	- User Themes
	- Dash to Dock

Open Tweak Tools

	- Appearance
		- Select GTK+ : OSX-Arc-Darker
		- Select Icons : EPapirus
		- Select Shell theme : Gnome-OSX-Dark-Shell
	- Windows
		- Enable Titlebar Buttons Mximize and Minimize
	- Extensions
		- click on the cog on Dash to dock
		- Position on screen : Bottom
		- Icon size limit : 32px
		- Intelligent autohide cog : 
			- Deactivate push to show
		- In appearance : Shrink the dash on, show windows counter indicators on, customize opacity on to 80%

Final touch, run this :

	gsettings set  org.gnome.desktop.wm.preferences button-layout 'close,minimize,maximize:'

## Usefull stuff

	sudo apt install -y vim terminator geary git

Open terminator and right click in the window -> Preferences -> Profiles
deactivate Show titlebar
Background -> transparent -> 80%

We can create a ssh key

	ssh-keygen -t rsa



