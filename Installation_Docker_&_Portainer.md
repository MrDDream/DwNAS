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


