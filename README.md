

Step 1: First, build a default-jwm .iso with this command...

	sudo ISO=jwm install-nutyx


Step 2: After it finishes building the basic .iso, if you want
 	to customize it, enter chroot with this command...

	sudo install-nutyx -ec



Step 3: Add the packages needed for your customization...

sudo cards install xdgmenumaker dmenu oxy-cursors deepin-gtk-theme      \
    pavucontrol picom ttf-liberation yad lxde-appearance \
    papirus-icon-theme pcmanfm leafpad volumeicon        \
    xfce4-notifyd conky nitrogen



Step 4: Move files, scripts, etc. into designated folders...

	Open the file manager as root, go to /mnt/hd/, and copy 
	files/folders from your system into the corresponding
	folders.

	**Modify "Desktop Preferences" desktop file in /mnt/hd/usr/share/applications/ so it won't show in the menu
  
	Copy the following from your files/folders into /mnt/hd/ folders...

		/root/.gtkrc-2.0
		/usr/share/images
		/etc/fonts/local.conf
		/etc/.bashrc

	**Copy these files/folders from the HOME folder into /mnt/hd/etc/skel/

		.conkyrc
		.gtkrc-2.0
		.jwmrc
		.Xresources
		.bashrc

	**Copy these files/folders from ~/.config/ into /mnt/hd/etc/skel/.config/

		conky 
		glib-2.0
		gtk-2.0
		gtk-3.0
		jwm
		libfm
		nitrogen
		pcmanfm
		volumeicon
		xfce4
		picom.conf

