# CheatSheet

Voici l'ensemble de mon aide-mémoire, appelé en anglais *cheatsheet*, classé par thème en ordre alphabétique après la partie concernant l'installation et la configuration de Kali :

1. [Installation et configuration de Kali](#installation_kali)

## Installation et configuration de Kali <a name="installation_kali"></a>

Je télécharge la machine virtuelle correspondant à VirtualBox : https://www.kali.org/get-kali/#kali-virtual-machines

Les identifiants de connexion par défaut sont : kali / kali  
Au premier lancement, le clavier étant en QWERTY, il faut taper : kqli

Dans un premier temps, dans un terminal, je configure temporairement le clavier en AZERTY avec la commande suivante : `setxkbmap fr`  
Ensuite, je configure la langue du système : `sudo dpkg-reconfigure locales`  
Puis je configure, cette fois-ci de manière permanente, le clavier : `sudo dpkg-reconfigure keyboard-configuration`  
Enfin, je configure l'horloge système : `sudo timedatectl set-timezone Europe/Paris`  
Je redémarre le système : `sudo reboot`  
Je mets à jour le système : `sudo apt update` puis `sudo apt upgrade`  
Je redémarre une seconde fois le système : `sudo reboot`  
Je purge les paquets qui ne sont plus nécessaires : `sudo apt autoremove`  
Je prends un instantané (aussi appelé *snapshoot* en anglais) de la machine virtuelle et tout est prêt !
