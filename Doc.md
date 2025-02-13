![body](https://banzaihobby.com/cdn/shop/files/Aoshima_Initial_D_Takumi_Fujiwara_AE86_Trueno_Project_D_Specification_-_BanzaiHobby-254450.jpg?v=1717061182&width=1100)

# Le Laboratoire

### **Somaire**

1. [Introduction](#introduction)

2. [Mise en place Serveur](#mise-en-place-serveur)

2.1 [RAID](#raid)

2.2 [ILO](#ilo)

2.3 [Proxmox](#proxmox)

3. [Mise en place Routeur](#mise-en-place-routeur)

3.1 [OPNSense](#opnsense)

3.2 [Configuration Switch](#configuration-switch)

4. [Mise en place Machine](#mise-en-place-machine)

4.1 [Debian 12](#debian-12)

4.2 [Windows 10](#windows-10)

4.3 [Windows 11](#windows-11)

4.4 [Atlas OS](#atlas-os)

4.5 [Ubuntu](#ubuntu)

5. [Autres](#autres)

6. [Test](#test)

## Introduction

> Tous les liens présents dans cette documentation sont sécurisés et ont été vérifiés par mes soins. Tu peux donc cliquer sans souci !

- [~] Expliquer le but de la doc et les différente partie

**Bonjour à toi, jeune lecteur de ma documentation,**

Ci-dessous, tu trouveras la plupart des mises en place que j'ai réalisées au cours de mes études.
Chaque installation sera détaillée au maximum, et une version traduite en anglais par mes soins sera également disponible.

Chaque début de chapitre te fournira les connaissances nécessaires sur le sujet abordé.
Cette documentation est disponible sur mon GitHub et sur mon site web.
Si tu souhaites proposer une modification ou donner ton avis, n'hésite pas à le faire sur ces plateformes.

## Mise en place Serveur

- [~] Expliquer ce qu'est un serveur, c'est composant et son utiliter ou utilisation

### **Qu'est-ce qu'un serveur ?**  

Un **serveur** est un ordinateur puissant ou un logiciel dédié qui fournit des services, des ressources ou des données à d'autres ordinateurs appelés **clients** via un réseau (comme Internet ou un réseau local). Son rôle principal est de répondre aux demandes des clients et de leur fournir les informations demandées.  

---

### **Les composants d'un serveur**  

Un serveur est composé de plusieurs éléments essentiels, similaires à ceux d'un ordinateur classique, mais avec des caractéristiques plus robustes pour assurer des performances élevées et une disponibilité continue :  

1. **Processeur (CPU)** :  
   - Cœur du serveur, il traite toutes les demandes et exécute les tâches.  
   - Souvent, les serveurs utilisent des processeurs multicœurs de haute performance pour gérer plusieurs requêtes simultanément.  

2. **Mémoire vive (RAM)** :  
   - Stocke temporairement les données en cours de traitement pour un accès rapide.  
   - Plus un serveur a de RAM, plus il peut gérer de demandes en même temps.  

3. **Stockage (Disques durs ou SSD)** :  
   - Conserve les données, les applications et le système d'exploitation.  
   - Les serveurs utilisent souvent des **RAID** pour sécuriser les données et améliorer les performances.  

4. **Carte réseau (NIC - Network Interface Card)** :  
   - Permet au serveur de communiquer avec d'autres appareils via un réseau.  
   - Des cartes réseau haut débit (1 Gbps, 10 Gbps, voire plus) sont utilisées pour des connexions rapides et fiables.  

5. **Alimentation redondante** :  
   - Pour garantir une disponibilité continue, les serveurs ont souvent plusieurs alimentations pour éviter les pannes en cas de défaillance d'une d'elles.  

6. **Système de refroidissement** :  
   - Les serveurs dégagent beaucoup de chaleur en raison de leurs composants performants, d'où l'importance d'un bon système de ventilation ou de refroidissement liquide.  

---

### **Utilité et utilisation des serveurs**  

Les serveurs ont de nombreuses utilisations dans divers domaines :  

1. **Serveurs Web** :  
   - Hébergent des sites web et fournissent des pages web aux navigateurs des utilisateurs.  
   - Exemples : Apache, Nginx.  

2. **Serveurs de fichiers** :  
   - Stockent et partagent des fichiers dans un réseau (documents, images, vidéos).  
   - Exemples : Serveurs NAS (Network Attached Storage).  

3. **Serveurs de bases de données** :  
   - Gèrent et stockent des bases de données pour des applications et des sites web.  
   - Exemples : MySQL, PostgreSQL, MongoDB.  

4. **Serveurs de messagerie** :  
   - Gèrent l'envoi, la réception et le stockage des e-mails.  
   - Exemples : Microsoft Exchange, Postfix.  

5. **Serveurs d'applications** :  
   - Hébergent et exécutent des applications logicielles utilisées par les clients.  
   - Exemples : Node.js, Apache Tomcat.  

6. **Serveurs de virtualisation** :  
   - Hébergent plusieurs machines virtuelles sur un seul serveur physique.  
   - Exemples : VMware ESXi, Hyper-V.  

7. **Serveurs de jeux** :  
   - Hébergent des sessions de jeux en ligne pour permettre à plusieurs joueurs de jouer ensemble.  

---

### **Conclusion**  

Les serveurs sont indispensables à l'infrastructure numérique moderne. Ils garantissent l'accès aux informations, le stockage sécurisé des données et l'exécution efficace des applications. Le choix du type de serveur et de ses composants dépend des besoins spécifiques de l'utilisateur ou de l'organisation.  

### RAID

- [ ] Gestion du raid et niveau
- [ ] Explication du montage raid depuis le serveur 
- [ ] Montage raid depuis debian 12

### ILO

Texte du chapitre 1.2 ici...

### Proxmox

Texte du chapitre 1.3 ici...

## Mise en place Routeur

- [~] Expliquer ce qu'est un routeur

### **Qu'est-ce qu'un routeur ?**  

Un **routeur** est un appareil réseau qui permet de connecter plusieurs réseaux entre eux et de diriger le trafic de données entre ces réseaux. Il joue un rôle essentiel dans la communication sur Internet en déterminant le meilleur chemin pour transmettre les données d'un expéditeur à un destinataire.  

En d'autres termes, un routeur agit comme un **chef d'orchestre** qui s'assure que les informations (comme les pages web, les e-mails ou les vidéos en streaming) arrivent à la bonne destination de manière rapide et efficace.  

---

### **Fonctionnement d'un routeur**  

Le routeur reçoit des **paquets de données** (petits blocs d'informations) d'un appareil (ordinateur, smartphone, tablette) et décide où les envoyer en fonction de leur **adresse IP de destination**.  
Il utilise pour cela une **table de routage**, qui contient les chemins possibles pour atteindre chaque destination. Le routeur choisit le chemin le plus rapide et le plus efficace pour transmettre les données.  

---

### **Les différents types de routeurs**  

1. **Routeurs domestiques** :  
   - Utilisés à la maison pour connecter plusieurs appareils à Internet via une connexion Wi-Fi ou par câble.  
   - Ils fournissent également des fonctionnalités de sécurité comme un pare-feu intégré.  

2. **Routeurs professionnels ou d'entreprise** :  
   - Utilisés dans les entreprises pour gérer de grands réseaux complexes.  
   - Ils offrent des fonctionnalités avancées comme le **VPN** (réseau privé virtuel), la gestion de la bande passante et une sécurité renforcée.  

3. **Routeurs sans fil (Wi-Fi)** :  
   - Permettent aux appareils de se connecter à Internet sans fil.  
   - Ils utilisent des normes Wi-Fi comme **Wi-Fi 5 (802.11ac)** ou **Wi-Fi 6 (802.11ax)** pour des connexions rapides et stables.  

4. **Routeurs de centre de données** :  
   - Utilisés dans les centres de données pour gérer d'énormes volumes de données.  
   - Ils offrent des vitesses très élevées et une redondance pour éviter les pannes.  

---

### **Les fonctions principales d'un routeur**  

1. **Acheminement des données** :  
   - Dirige les paquets de données vers leur destination en utilisant l'adresse IP.  

2. **Partage de connexion Internet** :  
   - Permet à plusieurs appareils de partager une seule connexion Internet.  

3. **Pare-feu et sécurité** :  
   - Protège le réseau contre les menaces externes en filtrant les paquets malveillants.  

4. **NAT (Network Address Translation)** :  
   - Masque les adresses IP privées des appareils connectés pour les protéger sur Internet.  

5. **DHCP (Dynamic Host Configuration Protocol)** :  
   - Attribue automatiquement des adresses IP aux appareils du réseau local.  

---

### **Utilité d'un routeur**  

- **À la maison** :  
  - Connecte tous les appareils (ordinateurs, smartphones, tablettes, télévisions) à Internet via Wi-Fi ou câble Ethernet.  
  - Offre une sécurité de base pour protéger le réseau domestique.  

- **En entreprise** :  
  - Gère de grands réseaux avec de nombreux appareils connectés.  
  - Optimise le flux de données pour assurer une connexion rapide et stable.  
  - Protège les données sensibles avec des pare-feu avancés et des VPN.  

- **Sur Internet** :  
  - Les routeurs font partie de l'infrastructure principale d'Internet, reliant des millions de réseaux dans le monde entier.  
  - Ils dirigent les données de manière efficace, garantissant que les informations arrivent rapidement à destination.  

---

### **En résumé**  

Un **routeur** est un appareil indispensable à la communication en réseau, que ce soit à la maison, en entreprise ou sur Internet. Il garantit une **connexion fluide, rapide et sécurisée** entre les appareils et permet de partager une connexion Internet de manière efficace.  

### OPNSense

- [ ] Gestion OPNSense et différente régle
- [ ] Installation et réglage option importante

### Configuration Switch

- [ ] Voir pour le changer de place mais ici pour le moment
- [ ] Expliquer la mise en place de vlan et leur utiliter
- [ ] Expliquer Minicom, comment l'intaller et l'utiliser

## Mise en place Machine

- [~] Expliquer ce qu'est un système d'exploitation et les différence entre chaqu'un si la foi est présente

### **Qu'est-ce qu'un ordinateur ?**  

Un **ordinateur** est une machine électronique capable de traiter, stocker et exécuter des instructions sous forme de programmes. Il permet de réaliser diverses tâches, comme naviguer sur Internet, écrire des documents, jouer à des jeux, gérer des bases de données, ou encore programmer.  

---

### **Les composants d'un ordinateur**  

Un ordinateur est constitué de plusieurs éléments matériels (hardware) et logiciels (software) qui travaillent ensemble :  

1. **Processeur (CPU - Central Processing Unit)** :  
   - C'est le **cerveau de l'ordinateur**. Il exécute les instructions des programmes et effectue les calculs nécessaires.  

2. **Mémoire vive (RAM - Random Access Memory)** :  
   - Stocke temporairement les données en cours de traitement pour un accès rapide.  
   - Plus il y a de RAM, plus l'ordinateur peut exécuter de tâches simultanément.  

3. **Stockage (Disque dur ou SSD)** :  
   - Conserve les données de manière permanente, comme le système d'exploitation, les logiciels et les fichiers personnels.  
   - Les **SSD (Solid State Drives)** sont plus rapides que les **disques durs (HDD)** traditionnels.  

4. **Carte graphique (GPU - Graphics Processing Unit)** :  
   - Gère l'affichage des images et des vidéos.  
   - Indispensable pour les jeux vidéo, le graphisme et l'édition vidéo.  

5. **Carte mère (Motherboard)** :  
   - Relie tous les composants entre eux et permet leur communication.  

6. **Périphériques** :  
   - **Entrée** : Clavier, souris, microphone, caméra.  
   - **Sortie** : Écran, imprimante, haut-parleurs.  

---

### **Qu'est-ce qu'un système d'exploitation ?**  

Un **système d'exploitation (OS - Operating System)** est un logiciel essentiel qui permet de gérer les ressources matérielles de l'ordinateur et de fournir une interface utilisateur pour exécuter des applications.  
Il agit comme un **intermédiaire** entre le matériel (hardware) et les logiciels (applications).  

**Fonctions principales d'un système d'exploitation** :  
- **Gestion des ressources** : Gère l'utilisation du processeur, de la RAM et du stockage.  
- **Gestion des fichiers** : Organise les fichiers et les dossiers sur le disque dur.  
- **Interface utilisateur** : Fournit un environnement graphique (comme le bureau, les icônes et les fenêtres) pour interagir avec l'ordinateur.  
- **Exécution des applications** : Permet de lancer et de gérer plusieurs applications simultanément.  
- **Sécurité** : Protège l'ordinateur contre les virus et les accès non autorisés.  

---

### **Les différents systèmes d'exploitation : Linux vs Windows**  

#### **1. Windows**  
- **Développé par** : Microsoft.  
- **Utilisation** : Grand public, entreprises, jeux vidéo, logiciels professionnels (comme la suite Adobe).  
- **Interface utilisateur** : Très conviviale, avec un **bureau**, un **menu Démarrer** et des **fenêtres** pour naviguer facilement.  
- **Compatibilité logicielle** : Très large, la plupart des logiciels commerciaux sont développés pour Windows.  
- **Sécurité** : Plus vulnérable aux virus et malwares, nécessitant l'utilisation d'antivirus.  
- **Exemples de versions** : Windows 10, Windows 11.  

---

#### **2. Linux**  
- **Développé par** : Communauté open-source.  
- **Utilisation** : Serveurs, développement logiciel, utilisateurs avancés, systèmes embarqués (comme les smartphones Android).  
- **Interface utilisateur** : Personnalisable selon la distribution (ex. : Ubuntu utilise GNOME, Linux Mint utilise Cinnamon).  
- **Compatibilité logicielle** : Moins de logiciels commerciaux, mais de nombreux logiciels libres et gratuits.  
- **Sécurité** : Très sécurisé grâce à sa structure en permissions d'utilisateur et à sa faible exposition aux virus.  
- **Exemples de distributions** :  
  - **Ubuntu** : Convient aux débutants, avec une interface conviviale.  
  - **Debian** : Stable et sécurisé, souvent utilisé sur les serveurs.  
  - **Arch Linux** : Pour les utilisateurs avancés, hautement personnalisable.  
  - **Fedora** : Utilisé par les développeurs pour tester des logiciels récents.  

---

### **Différences entre Linux et Windows**  

| Critère            | **Windows**                            | **Linux**                               |
|-------------------|----------------------------------------|------------------------------------------|
| **Coût**           | Payant (licences Microsoft)             | Gratuit (open-source)                     |
| **Personnalisation**| Limitée aux paramètres du système      | Très personnalisable (interfaces, thèmes) |
| **Logiciels**      | Compatible avec la majorité des logiciels commerciaux | Principalement des logiciels libres, certains logiciels commerciaux via des émulateurs (Wine) |
| **Sécurité**       | Plus vulnérable aux virus               | Très sécurisé grâce à sa structure de permissions |
| **Performances**   | Exigeant en ressources pour les versions récentes | Léger et performant même sur du matériel ancien |
| **Utilisation**    | Grand public, entreprises, jeux vidéo   | Développement, serveurs, utilisateurs avancés |

---

### **En résumé**  
- Un **ordinateur** est une machine qui exécute des instructions grâce à son matériel (CPU, RAM, stockage, etc.).  
- Un **système d'exploitation** gère le matériel et fournit une interface pour utiliser des applications.  
- **Windows** est convivial, compatible avec de nombreux logiciels commerciaux, mais payant et plus vulnérable aux virus.  
- **Linux** est gratuit, sécurisé, hautement personnalisable, mais demande parfois plus de compétences techniques.  

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
