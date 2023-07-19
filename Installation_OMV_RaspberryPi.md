## B) Installation sur un Raspberry PI 4.

## Préparation de votre carde microSD :
1. Téléchargez [RPI Imager](https://www.raspberrypi.com/software/) (il s'agit du logiciel officiel de la Fondation Raspberry Pi)
2. Insérez votre microSD dans votre PC
3. Lancez Raspberry Pi Imager
4. Dans **"Système d'exploitation"**, choissisez ***"Raspberry Pi OS (other)"*** puis ***"Raspberry Pi OS (64-bit)"***
5. Sélectionnez votre microSD dans la partie **"Stockage"**
6. Cliquez sur l'engrenage en bas à droite du logiciel puis cochez :
   
   * Nom d'hôte (Il s'agit du nom de votre raspberry sur le réseau)
   * Activer SSH (Pour pouvoir prendre la main à distance sur votre réseau)
   * Définir nom d'utilisateur et mot de passe (Il s'agit du compte administrateur / root pour votre machine)
   * Configuré le Wi-Fi (pas nécessaire si vous comptez brancher votre RPI en filaire)
   * Définir les réglages locaux (Fuseau horaire Europe/Paris et type de clavier FR pour l'AZERTY)
7. Cliquez sur **"Ecrire"** et patientez.
8. Insérez votre microSD et branchez votre Raspberry Pi.

## Installation du système :

Connectez-vous à votre Raspberry avec le nom d'utilisateur et mot de passe renseigner à l'étape 6, puis tapez les commandes suivantes :

Vérifiez et mettre à jour votre RPI :
```
sudo apt update && sudo apt upgrade
```
Copiez la commande pour lancer le script d'installation d'OMV avec ses dépendances et OMV-extras :
```
wget -O - https://github.com/OpenMediaVault-Plugin-Developers/installScript/raw/master/install | sudo bash
```
Après cela votre Raspberry PI redémarrera à la fin du démarrage vous devriez voir cela :

![image](https://github.com/MrDDream/Home_NAS/blob/main/Images/Ecran_install_omv_desktop_final.png)

Ouvrez un navigateur internet (ex: Google Chrome) sur votre PC et renseignez l'adresse IP (ici encadré en rouge), vous devriez arriver sur cette page:

**Nom d'utilisateur :** admin

**Mot de passe :** openmediavault

![image](https://github.com/MrDDream/Home_NAS/blob/main/Images/OMV_GUI.png)

Pour utiliser votre compte précédemment crée comme administrateur d'OMV, allez dans la partie **"Utilisateur"** et modifié votre compte en ajoutant le groupe ***"openmediavault-admin"***
