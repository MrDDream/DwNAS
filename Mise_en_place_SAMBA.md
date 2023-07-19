 # Mise en place SAMBA (Partage de fichiers) :

 ## Activez le service SAMBA :

 1. Connectez-vous à la page Web de votre OpenMediaVault (http://192.168.X.X).
 2. Allez dans **"Services"** puis **"SMB/CFIS"**.
 3. Dans **"Paramètres"** sélectionnez **"Activé"** (Vous pouvez aussi activer les répertoires personnels et la corbeille).

 4. Puis cliquez sur **"Enregistrer"** en bas à droite de la page.

## Crée votre "système de fichiers" :

1. Allez dans le menu **"Stockage"** puis **"Systèmes de fichiers"**.
2. Cliquez sur le petit **"+"** et sélectionnez **"Créer"**.
3. Dans **"Périphérique"** sélectionnez votre HDD *(disque dur)* prévu pour le stockage en **"Type"** je vous recommande le **"EXT4"** et cliquez sur **"Enregistrer'**
   (l'opération peut-être plus ou moins longue selon la taille de votre disque dur).
4. Ensuite vous devriez être dans le menu **"Monter"**, sélectionnez pour **"Système de fichiers"** votre disque, il devrait s'appeller **/dev/sdb1**,
   pour le **"Seuil d'avertissement d'utilisation"** libre à vous de chosir le pourcentage.

5. Cliquez sur **"Enregister"**

Si tout c'est bien passer vous devriez voir ça :

![image](https://github.com/MrDDream/Home_NAS/blob/main/Images/Montage_OMV_HDD.png)

## Crée ses premiers dossiers partagés :

1. Allez dans le menu **"Stockage"** puis **"Dossiers partagés"**.
2. Cliquez sur le petit **"+"**
3. Vous avez maintenant plusieurs champs à renseigner :
   * **Nom** : le nom de votre partage, c'est pour vous reperez sur OMV.
   * **Système de fichiers** : votre disque monté précédemment.
   * **Chemin relatif** : le chemin de votre dossier partagé (exemple: Dossier1/, si vous compter crée un partage dans un partage, cela fera Dossier1/Dossier2/).
   * **Permissions** : selon votre besoin et qui y accède.
   * **Commentaire** : sans commentaire
  
4. Cliquez sur **"Enregistrer"**.
