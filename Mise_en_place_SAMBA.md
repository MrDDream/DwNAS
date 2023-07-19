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
