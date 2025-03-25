![body](https://banzaihobby.com/cdn/shop/files/Aoshima_Initial_D_Takumi_Fujiwara_AE86_Trueno_Project_D_Specification_-_BanzaiHobby-254450.jpg?v=1717061182&width=1100)

# 🔌 **Qu'est-ce qu'un Switch ?**  

- [Le Laboratoire 🔬](/Docs.md)

Un **switch** (ou commutateur réseau) est un équipement **réseau** qui permet de :  
- 🔗 **Connecter plusieurs appareils** (ordinateurs, serveurs, imprimantes, caméras IP) au sein d'un réseau local (**LAN**).  
- 🚀 **Transférer efficacement les données** entre ces appareils en identifiant le destinataire précis grâce aux **adresses MAC**.  
- ⚡ Optimiser la **bande passante** en envoyant les données uniquement à l'appareil concerné, contrairement à un **hub** qui diffuse les données à tous les ports.  

---

### ⚙️ **Comment fonctionne un Switch ?**  

1. **Table d'adresses MAC** 📜 :  
   - Le switch utilise une **table d'adresses MAC** pour savoir quel appareil est connecté à quel port.  
   - Lorsqu'un appareil envoie des données, le switch enregistre l'**adresse MAC** de l'expéditeur et le **port** associé.  

2. **Transmission des données** 📡 :  
   - Lorsque des données sont reçues, le switch :  
     - 🔍 Vérifie l'**adresse MAC** de destination.  
     - 📂 Consulte sa **table d'adresses MAC** pour trouver le port de destination.  
     - 🎯 **Envoie les données** uniquement sur ce port, garantissant ainsi **confidentialité** et **performance**.  

3. **Apprentissage et filtrage** 🤖 :  
   - Le switch **apprend automatiquement** les adresses MAC des appareils connectés.  
   - Si l'adresse de destination n'est pas connue, il diffuse le message à **tous les ports** (sauf celui de l'expéditeur), puis met à jour sa table après avoir reçu la réponse.  

---

### 🔄 **Types de Switchs**  

1. **Switch non manageable (Unmanaged Switch)** 🏠  
   - 🔌 **Plug-and-play** : Pas de configuration nécessaire.  
   - 🏢 Utilisé dans les **petits réseaux domestiques** ou les **petites entreprises**.  
   - 🚫 Aucune fonctionnalité avancée (pas de VLAN, QoS, monitoring).  
   - 💰 Moins coûteux et facile à installer.  

2. **Switch manageable (Managed Switch)** 🖥️ 
   - ⚙️ **Paramétrable** via une interface web, une ligne de commande (CLI) ou un protocole de gestion (SNMP).  
   - Permet :  
     - 🏗️ La **configuration des VLAN** pour isoler le trafic réseau.  
     - 📶 La **priorisation du trafic (QoS)** pour des applications critiques (voix, vidéo).  
     - 👀 La **surveillance** et l'**analyse du trafic réseau**.  
     - 🔐 Des **options de sécurité avancées** (listes de contrôle d'accès, authentification).  
   - 🏢 Utilisé dans les **réseaux d'entreprise**, les **datacenters** et les **environnements complexes**.  

3. **Switch empilable (Stackable Switch)** 📚
   - 🏗️ Plusieurs switchs peuvent être **empilés** (connectés entre eux) pour fonctionner comme un **seul switch logique**.  
   - 🎛️ Simplifie la gestion en **centralisant l'administration**.  
   - 🔄 Offre une **haute disponibilité** et une **extensibilité** en ajoutant simplement de nouveaux switchs à la pile.  

4. **Switch PoE (Power over Ethernet)** ⚡
   - 🔌 Fournit à la fois **l'alimentation électrique** et **la connexion réseau** via un seul câble Ethernet.  
   - 📹 Idéal pour les **caméras IP**, les **téléphones VoIP** et les **points d'accès Wi-Fi**.  
   - ✅ Conforme aux normes **PoE (IEEE 802.3af)** et **PoE+ (IEEE 802.3at)** pour fournir plus de puissance.  

---

### 🛠️ **Fonctionnalités avancées des Switchs manageables**  

1. **VLAN (Virtual LAN)** 🌐 
   - Permet de **segmenter le réseau** en plusieurs sous-réseaux logiques pour :  
     - 🔒 **Isoler le trafic** (ex : réseau invité, réseau administratif).  
     - 🚀 Améliorer la **sécurité** et la **performance**.  

2. **QoS (Quality of Service)** 🚦 
   - 📊 Priorise le **trafic réseau critique** (ex : VoIP, streaming vidéo) pour éviter les **latences** et garantir la **qualité de service**.  

3. **Link Aggregation (LACP)** 🔗 
   - ⚡ Combine plusieurs **ports réseau** pour créer un **lien unique à haute bande passante**.  
   - 🛡️ Offre une **redondance** en cas de défaillance d'un port.  

4. **Spanning Tree Protocol (STP)** 🔄 
   - 🚫 **Évite les boucles réseau** en désactivant automatiquement les liens redondants.  
   - 🔄 Garantit la **stabilité du réseau** dans des topologies complexes.  

5. **Port Mirroring** 🎥 
   - 👀 **Copie le trafic réseau** d'un port vers un autre pour l'**analyse** ou le **débogage**.  
   - 🛠️ Utilisé pour la **surveillance du réseau** avec des outils comme **Wireshark**.  

6. **Sécurité réseau** 🔐 
   - 🛑 **Listes de contrôle d'accès (ACL)** pour filtrer le trafic.  
   - 🔑 **Authentification 802.1X** pour vérifier l'identité des appareils connectés.  
   - 🦠 **Protection contre les attaques** (ex : storm control, DHCP snooping).  

---

### 🏢 **Exemples d'utilisation**  

- 🏠 **Réseaux domestiques** : Pour connecter des ordinateurs, consoles de jeux, télévisions connectées.  
- 🏢 **Petites entreprises** : Pour interconnecter des postes de travail, des serveurs, des imprimantes.  
- 🏭 **Datacenters** : Utilisation de **switchs empilables** et **manageables** pour des réseaux haute disponibilité.  
- 🏬 **Bureaux partagés** : Utilisation de **VLAN** pour isoler le trafic des différentes équipes.  
- 🏢 **Bâtiments connectés** : Utilisation de **PoE** pour alimenter des caméras de sécurité, des points d'accès Wi-Fi.  

---

### 📊 **Comparaison avec d'autres équipements réseau**  

| **Équipement** | **Fonction principale**                        | **Différence avec un Switch**                       |
|----------------|------------------------------------------------|----------------------------------------------------|
| **Hub 📡**        | Diffuse les données à tous les ports            | Moins intelligent, pas de table MAC, moins sécurisé |
| **Routeur 🌍**    | Connecte différents réseaux (ex : LAN à Internet) | Le switch connecte des appareils **au sein d'un même réseau** |
| **Point d'accès Wi-Fi 📶** | Fournit une connexion Wi-Fi aux appareils sans fil | Le switch connecte des appareils **filaire**        |
| **Pare-feu 🔥**   | Protège le réseau contre les menaces externes   | Le switch ne filtre pas le trafic (sauf ACL avancées) |

---

### 🎯 **En résumé**  
- Un **switch** est un élément essentiel d'un réseau local pour **connecter et acheminer efficacement** les données entre plusieurs appareils.  
- Il utilise une **table d'adresses MAC** pour **envoyer les données uniquement à l'appareil concerné**, offrant ainsi **sécurité**, **performance** et **efficacité**.  
- Il existe plusieurs types de switchs :  
  - **Non manageable** : Simple à utiliser mais sans fonctionnalités avancées.  
  - **Manageable** : Personnalisable avec des fonctions avancées (VLAN, QoS, sécurité).  
  - **Empilable** : Pour les grands réseaux avec haute disponibilité.  
  - **PoE** : Pour alimenter des appareils réseau via Ethernet.  
- **Les switchs manageables** sont recommandés pour les réseaux professionnels nécessitant **sécurité**, **performance** et **flexibilité**.  

---
- [Le Laboratoire 🔬](/Docs.md)

Texte du chapitre ici...