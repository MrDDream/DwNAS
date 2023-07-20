# 3) Installation de Docker & Portainer

## Installation de Docker :

1. Connectez-vous en SSH à votre système (vous pouvez utiliser **"Terminal Windows"**, **"Putty"** ou d'autres outils).
   
3. Connectez-vous en Root (super utilisateur):
```
sudo su
```
4. Ajoutez le repository Docker officiel.
```
sudo apt update
sudo apt install ca-certificates curl gnupg
```
```
sudo install -m 0755 -d /etc/apt/keyrings
curl -fsSL https://download.docker.com/linux/debian/gpg | sudo gpg --dearmor -o /etc/apt/keyrings/docker.gpg
sudo chmod a+r /etc/apt/keyrings/docker.gpg
```
```
echo \
  "deb [arch="$(dpkg --print-architecture)" signed-by=/etc/apt/keyrings/docker.gpg] https://download.docker.com/linux/debian \
  "$(. /etc/os-release && echo "$VERSION_CODENAME")" stable" | \
  sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
```
5. Installez Docker :
```
sudo apt update
```
```
sudo apt install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
```
Docker est maintenant installer et vous pouvez désormer utilisé les commandes **"docker"**.

## Installation de Portainer :

1. Création d'un **"volume"** pour Portainer (son stockage):
```
docker volume create portainer_data
```
2. Création du container Portainer:
```
docker run -d -p 8000:8000 -p 9443:9443 --name portainer --restart=always -v /var/run/docker.sock:/var/run/docker.sock -v portainer_data:/data portainer/portainer-ce:latest
```
3. Ouvrez un navigateur Web et tapez "https://192.168.1.X:9443" (renseignez votre IP), vous devriez tomber sur cette page :

![image](https://github.com/MrDDream/Home_NAS/blob/main/Images/Portainer_first.png)

4. Renseignez l'identifiant et le mot de passe que vous souhaitez.

Vous devriez arriver sur la page **"Home"** de Portainer comme cela :

![image](https://github.com/MrDDream/Home_NAS/blob/main/Images/Portainer_home.png)

Félictation vous pouvez maintenant passez à l'étape concernant la création de Container [ICI](https://github.com/MrDDream/Home_NAS/blob/main/Creation_container_via_portainer.md).

