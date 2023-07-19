# A) Installation sur un ordinateur de bureau.

## Préparation de la clé d'installation :
1. Téléchargez la dernière version de l'ISO sur le site officiel [ICI](https://www.openmediavault.org/download.html). 
3. Téléchargez [Rufus](https://rufus.ie/fr/) (c'est un logiciel permettant la création de clé USB bootable). 
4. Connectez votre clé USB.
5. Lancez Rufus, puis cliquez sur **"Sélection"** et séléctionnez votre fichier ISO.
6. Cliquez sur **"Démarrer"** et patientez *(vous devriez avoir un message vous indiquant que votre clé va être effacée, cliquez sur OK, si vous n'avez rien à perdre sur cette dernière)*

## Installation du système :

Pour commencer branchez votre clé USB sur le PC qui va acceuillir le NAS, allumez votre PC et ***booter*** sur votre clé en appuyant sur la bonne touche (tapez "touche boot *marque de votre PC* sur Google pour trouver celle qui ccorespond à votre PC).

*Si vous rencontrez des difficultés pour boot sur votre clé USB, vérifiez que le ***Secure Boot*** n'est pas activé sur votre machine.*

Si tout ce passe bien vous devriez voir cette écran :

![image](https://github.com/MrDDream/Home_NAS/blob/main/Images/Ecran_install_omv_desktop.png)

1. Faites **"Entrée"** pour lancer l'installation.
2. Sélectionnez votre Langue
3. Sélectionnez votre Pays
4. Sélectionnez la dispostion de votre Clavier (Français = AZERTY, Anglais = QWERTY)
5. Pour le **"Nom de machine"**, renseignez un nom pour vous (c'est le nom avec lequel il apparaîtra sur votre réseau).
6. Pour le **"Domaine"** laissez *"local"* par défaut.
7. Pour le mot de passe **superutilisateur** (ou root), renseignez un mot de passe assez complexe, il s'agit du mot de passe "administrateur" de votre machine.
8. Confirmez votre mot de passe **root**
9. **"Configurer l'outil de gestion des paquets"**, sélectionnez ***"France"*** puis ***"deb.debian.org"*** (dépôt officiel).
10. Laissez la partie ***"Mendataire HTTP"*** vide et continuez.
11. Pour l'installation du ***"GRUB"*** sélectionnez le disque où est installé votre système.

Vous devriez maintenant être sur l'écran ***"Terminer l'installation"*** faites **"Continuer"** votre machine va redémarrer.

Après redémarrage votre écran devrez ressembler à ça : (l'encadré rouge correspond à l'adresse IP actuelle de votre machine)

![image](https://github.com/MrDDream/Home_NAS/blob/main/Images/Ecran_install_omv_desktop_final.png)

## Première connexion :

Ouvrez un navigateur internet (ex: Google Chrome) et tapez l'adresse indiqué (pour moi, il s'agit de 192.168.1.33), vous devriez arriver sur cette page :

![image](https://github.com/MrDDream/Home_NAS/blob/main/Images/OMV_GUI.png)


