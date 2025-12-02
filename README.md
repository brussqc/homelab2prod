# Explication du homelab2prod

## Composantes physiques

- HP Prodesk avec comme OS Debian 13. Il fait office de machine serveur et serveur gitolite. C'est lui qui fait les push sur GitHub.
- Dell avec comme OS OpnSense. [Voir ce vidéo à 18:19 pour un tutoriel facile à suivre pour l'installation] (https://www.youtube.com/watch?v=vJBoCgptF-0)
- Une [switch Unifi] (https://ca.store.ui.com/ca/en/category/switching-utility/products/usw-lite-8-poe)

## Explication du réseau
! [Réseau du homelab2 de noumanity] (schemanoumanity.jpg)

- STEVE aka la machine serveur administre le serveur gitolite. Il est branché en LAN dans la switch. Ici on ne voit que STEVE mais toutes autres connections dans la switch font partis du même réseau local (LAN).

- La switch est branchée dans le Dell qui lui est le Firewall OpnSense. En suivant la configuration automatique de OpnSense, j'ai assigné la connection de la switch comme LAN et la connection au modem comme WAN. En branchant un ordinateur à la switch, je peux maintenant aller sur le GUI de OpenSense à partir d'un navigateur web à l'adresse 192.168.1.1



