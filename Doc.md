![body](https://banzaihobby.com/cdn/shop/files/Aoshima_Initial_D_Takumi_Fujiwara_AE86_Trueno_Project_D_Specification_-_BanzaiHobby-254450.jpg?v=1717061182&width=1100)

# Le Laboratoire

**Somaire**

1. [Introduction](#introduction)
2. [Mise en place Serveur](#mise-en-place-serveur)
2.1. [RAID](#raid)
2.2. [ILO](#ilo)
2.3. [Proxmox](#proxmox)
3. [Mise en place Routeur](#mise-en-place-routeur)
3.1. [OPNSense](#opnsense)
3.2. [Configuration Switch](#configuration-switch)
4. [Mise en place Machine](#mise-en-place-machine)
4.1. [Debian 12](#debian-12)
4.2. [Windows 10](#windows-10)
4.3. [Windows 11](#windows-11)
4.4. [Atlas OS](#atlas-os)
4.5. [Ubuntu](#ubuntu)
5. [Autres](#autres)
6. [Test](#test)

## Introduction

> Tout type de lien présent dans cette doc son sécurisé et vérifier par mes soins donc pas de soucis tu peux cliquer ;)

- [ ] Expliquer le but de la doc et les différente partie

## Mise en place Serveur

- [ ] Expliquer ce qu'est un serveur, c'est composant et son utiliter ou utilisation

### RAID

- [ ] Gestion du raid et niveau
- [ ] Explication du montage raid depuis le serveur 
- [ ] Montage raid depuis debian 12

### ILO

Texte du chapitre 1.2 ici...

### Proxmox

Texte du chapitre 1.3 ici...

## Mise en place Routeur

- [ ] Expliquer ce qu'est un routeur

### OPNSense

- [ ] Gestion OPNSense et différente régle
- [ ] Installation et réglage option importante

### Configuration Switch

- [ ] Voir pour le changer de place mais ici pour le moment
- [ ] Expliquer la mise en place de vlan et leur utiliter
- [ ] Expliquer Minicom, comment l'intaller et l'utiliser

## Mise en place Machine

- [ ] Expliquer ce qu'est un système d'exploitation et les différence entre chaqu'un si la foi est présente

### Debian 12

>Pour une bonne install et connexions présente prendre la netinst sinon DVD en hors réseaux mais il y aura quelque petit problème de paquet.

- [ ] Gestion Paquet et Outils Utile
- [ ] Etape Installation et bonne pratique

### Windows 10

> Pas de manipulation particulière pour l'installation car l'option compte local est un choix encore disponible dans cette version.

- [ ] Outils Utile (et gestion du dualboot si besoin ou utile)
- [ ] Etape Installation sans connexion
- [ ] Etape Installation avec connexion (suppréssion des merdes installer a cause de la connexion)

### Windows 11

>Pour une install sans connexion et avec un compte local ouvrir l'invite de commande avec `control + F10` suivie de la commande `$ oobe\bypassnro` cela aura pour effet de redémarrer l'installation depuis la première question mais rajoutera la petite option sans connection lors de la demande de connection a votre compte microsoft.

- [ ] Outils Utile (et gestion du dualboot si besoin ou utile)
- [ ] Etape Installation sans connexion
- [ ] Etape Installation avec connexion (suppréssion des merdes installer a cause de la connexion)

### Atlas OS

- [ ] Etape d'installation Windows 10
- [ ] Etape d'installation Windows 11

### Ubuntu

- [ ] Gestion Paquet et Outils Utile
- [ ] Etape Installation et bonne pratique

## Autres

- Pare-Feu (Routeur mais a reconfirmer et si c'est le cas alors le mettre dans le bon chapitre)
- Service SSH
- Serveur Web
- VMWare et HyperV
- Les plages IP et les bonnes pratiques (10.X.X.X/24 ou /8)
- Schéma réseaux
- Médicat (super pour faire joue joue avec plein de logicil)
- Ventoy et autre logiciel pour clés boot
- Ou trouver des ISO (bon site ou autre) [Liens](https://lecrabeinfo.net/telecharger/)
- Petit tips logiciel sympa ou utile a installer (navigateur et autre)
- Voir pour complété quand idée ou nouveau cours ou nouvelle découverte

## Test

<s> test </s>

    <?php
        echo "Hello world!";
    ?>
