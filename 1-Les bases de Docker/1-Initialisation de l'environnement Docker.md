# résumé.
>Docker est la principale plateforme de conteneurisation. Si vous utilisez des conteneurs, vous utilisez probablement Docker.
- Pour travailler avec Docker, vous devez disposer du démon Docker et de la CLI..
- Cet atelier vous apprend à configurer votre environnement, afin que vous puissiez commencer à travailler avec Docker dès aujourd'hui ! 


## Contenu
* [SSH to your EC2 Instance](#ssh-to-your-ec2-instance)
* [Installation de Docker](#)
* [Activer le deamon Docker](#)
* [Executer une image test](#)


## SSH to your EC2 Instance
- Vos Credentials et IP respectives vous seront envoyés sur le chat
- Une clé SSH .pem vous sera transmise sur le chat
- username : `ec2-user`
- adresse ip : `adresse ip fournie`
- Se rendre dans le repertoire où vous  avez mis votre fichier pem
  Par exemple, si vous êtes sur windows et que vous l'avez mis dans le dossier téléchargements :

```
cd downloads
```
- et puis connectez-vous à l'instance EC2 :

```
ssh -i "cle-ssh.pem" ec2-user@ec2-addresse_ip.compute-1.amazonaws.com
```

## Installation de Docker

```
sudo yum -y install docker
```

## Activer le deamon Docker

```
sudo systemctl enable --now docker
```


## Executer une image test

```
docker run hello-world
```