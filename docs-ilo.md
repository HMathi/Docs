![body](https://banzaihobby.com/cdn/shop/files/Aoshima_Initial_D_Takumi_Fujiwara_AE86_Trueno_Project_D_Specification_-_BanzaiHobby-254450.jpg?v=1717061182&width=1100)
## **Qu'est-ce que l'iLO ?**  

L'**iLO (Integrated Lights-Out)** est une technologie de gestion à distance des serveurs développée par **Hewlett Packard Enterprise (HPE)**.  
Elle permet aux administrateurs système de :  
- **Superviser, gérer et dépanner** les serveurs à distance, même si le système d'exploitation principal est hors service.  
- **Accéder à l'interface du serveur** comme s'ils étaient physiquement devant lui, grâce à une console distante.  

L'iLO est intégré directement sur la **carte mère** des serveurs HPE et fonctionne indépendamment du système d'exploitation installé sur le serveur.  

---

### **Fonctionnalités principales de l'iLO**  

1. **Accès à distance** :  
   - Permet de contrôler le serveur via une console distante accessible depuis un navigateur web.  
   - Émule l'écran, le clavier et la souris du serveur (fonction **KVM - Keyboard Video Mouse**).  

2. **Supervision du matériel** :  
   - Surveille l'état des composants matériels : processeur, mémoire, alimentation, température, ventilateurs.  
   - Envoie des alertes en cas de défaillance matérielle ou de problème critique.  

3. **Gestion de l'alimentation** :  
   - Permet de **démarrer, arrêter et redémarrer** le serveur à distance.  
   - Accès aux fonctions avancées comme l'**arrêt forcé** ou le **redémarrage en mode maintenance**.  

4. **Accès au BIOS/UEFI** :  
   - Accès à distance au **BIOS/UEFI** du serveur pour modifier les paramètres système sans intervention physique.  

5. **Gestion des supports virtuels** :  
   - Monte des **supports virtuels** (ISO, disques distants) comme s'ils étaient connectés physiquement au serveur.  
   - Pratique pour **installer un système d'exploitation à distance**.  

6. **Sécurité avancée** :  
   - Authentification par mot de passe, **certificats SSL**, intégration avec **Active Directory** pour un accès sécurisé.  
   - Journalisation des actions effectuées pour un suivi des activités administratives.  

---

### **Versions de l'iLO**  

HPE a développé plusieurs versions de l'iLO au fil du temps :  
- **iLO 2** : Fonctions de base pour la gestion à distance des anciens serveurs HPE.  
- **iLO 3** : Améliorations en matière de performances et de sécurité.  
- **iLO 4** : Fonctionnalités avancées de gestion et de surveillance, y compris le support HTML5.  
- **iLO 5** : La version la plus récente avec une interface utilisateur modernisée, un **accès KVM amélioré** et des fonctionnalités de **sécurité renforcée** (comme la détection de firmware compromis).  

---

### **iLO : Version gratuite vs Version payante**  

- **iLO Standard (gratuit)** :  
  - Fonctions de base : Surveillance du matériel, gestion de l'alimentation, accès au BIOS/UEFI.  
  - Accès à distance limité (pas de KVM ni de supports virtuels).  

- **iLO Advanced (payant)** :  
  - Accès **KVM complet** avec console distante en temps réel.  
  - **Supports virtuels** pour installer des systèmes d'exploitation à distance.  
  - Fonctionnalités de **sécurité avancée** et d'**analyse des performances**.  

---

### **Avantages de l'iLO**  
- **Gestion centralisée** : Permet de gérer plusieurs serveurs à partir d'une seule interface.  
- **Gain de temps** : Les administrateurs peuvent effectuer des interventions sans se déplacer physiquement.  
- **Sécurité accrue** : Contrôle d'accès sécurisé avec journalisation des actions.  
- **Réduction des interruptions de service** : Diagnostic et dépannage à distance pour un **temps de rétablissement plus rapide**.  

---

### **Limitations de l'iLO**  
- **Coût** : Les fonctionnalités avancées nécessitent une **licence payante**.  
- **Complexité** : Configuration réseau et sécurité plus complexes à gérer dans un environnement multi-sites.  
- **Compatibilité** : Exclusivement disponible sur les **serveurs HPE**.  

---

### **En résumé**  
- **iLO** est un outil puissant pour la gestion à distance des serveurs HPE.  
- Il permet d'effectuer des tâches d'administration, de surveillance et de dépannage, même si le système d'exploitation principal ne fonctionne pas.  
- La version **gratuite** offre des fonctionnalités de base, tandis que la version **payante (iLO Advanced)** permet un accès complet à distance (KVM, supports virtuels, sécurité avancée).  

---

### **Comment accéder a l'ILO au demarrage du Serveur ?**

> Exemple et explication ci-dessous pour un serveur HP de 2019

1. Allumer le serveur
2. 

Texte du chapitre ici...