# Création d'un NAS maison
Tutoriel pour la création d'un NAS (Network Attached Storage) maison.

## Prérequis :
* Ordinateur de bureau (ou RPI 4, minimum 4Go de RAM).
* Clé USB 8Go minimum (Adaptateur micro-USB pour RPI).
* Connexion Internet (filaire de préférence).

_Je vous conseille un petit SSD pour l'installation de votre système et un HDD de grande capacité pour vos données._

# 1) Installation d'OpenMediaVault (OMV)
Il s'agit d'une solution _"clés en mains"_ pour la création d'un NAS personnel (il existe d'autre solution comme TrueNAS par exemple).

_Leur site officiel: https://www.openmediavault.org/_
  ### [A) Installation sur un ordinateur de bureau.](https://github.com/MrDDream/Home_NAS/blob/main/Installation_OMV_Desktop.md)
  ### B) Installation sur un Raspberry PI 4.

# 2) Mise en place SAMBA (Partage de fichiers)
Permet la création de dossiers partagés entre votre NAS et vos apparails (Windows, Android etc...).

# 3) Installation de Docker & Portainer
Permet la mise en place de container permettant pas mal de choses, notamment la création d'un serveur multimédia.

# 4) Création de container via Portainer
Quelques explications sur l'utilisation de Portainer et Docker-compose.
