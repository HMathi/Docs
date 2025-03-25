![body](https://banzaihobby.com/cdn/shop/files/Aoshima_Initial_D_Takumi_Fujiwara_AE86_Trueno_Project_D_Specification_-_BanzaiHobby-254450.jpg?v=1717061182&width=1100)
# 💾 **Qu'est-ce que le RAID ?**  

- [Le Laboratoire 🔬](/Docs.md)

Le **RAID (Redundant Array of Independent Disks)** est une technologie qui permet de combiner plusieurs disques durs ou SSD pour :  
- **Améliorer les performances** (vitesse de lecture et/ou d'écriture)  
- **Assurer la redondance des données** (sécurité en cas de panne d'un disque)  
- **Augmenter la capacité de stockage**  

Le RAID est couramment utilisé dans les serveurs, les stations de travail et les systèmes de stockage pour garantir la **continuité du service** et **minimiser les risques de perte de données**.  

---

### 📊 **Les niveaux de RAID les plus courants**  

Il existe plusieurs niveaux de RAID, chacun ayant ses avantages et ses inconvénients. Voici les plus utilisés :  

---

### **1. RAID 0 (Entrelacement - Striping)** ⚡
- **Principe** : Les données sont réparties sur plusieurs disques (entrelacement).  
- ✅ **Avantages** :  
  ✔️ **Haute performance** : Lecture et écriture très rapides car les données sont lues et écrites simultanément sur tous les disques.  
  ✔️ **Capacité totale** : La capacité totale est égale à la somme des capacités de tous les disques.  
- ❌ **Inconvénients** :  
  ⚠️ **Aucune redondance** : Si un disque tombe en panne, **toutes les données sont perdues**.  
- **Utilisation** : Montage vidéo, jeux vidéo, où la performance est prioritaire par rapport à la sécurité des données.  
- **Nombre minimum de disques 💾** : 2  

---

### **2. RAID 1 (Miroir - Mirroring)** 🔍
- **Principe** : Les données sont **dupliquées** sur deux disques.  
- ✅ **Avantages** :  
  ✔️ **Redondance totale** : Si un disque tombe en panne, l'autre contient une copie exacte des données.  
  ✔️ **Lecture rapide** : Les données peuvent être lues simultanément sur les deux disques.  
- ❌ **Inconvénients** :  
  ⚠️ **Capacité réduite** : La capacité totale est celle d'un seul disque, car chaque donnée est copiée en double.  
- **Utilisation** : Données critiques nécessitant une haute sécurité, comme des bases de données financières.  
- **Nombre minimum de disques 💾** : 2  

---

### **3. RAID 5 (Parité distribuée - Distributed Parity)** 🛡️
- **Principe** : Les données sont réparties sur plusieurs disques avec une **parité** (informations de vérification) également répartie sur tous les disques.  
- ✅ **Avantages** :  
  ✔️ **Équilibre entre performances et sécurité** : Lecture rapide et protection contre la perte d'un disque.  
  ✔️ **Capacité optimisée** : La capacité totale est égale à la somme des disques moins un (utilisé pour la parité).  
- ❌ **Inconvénients** :  
  ⚠️ **Reconstruction lente** : Si un disque tombe en panne, le temps de reconstruction est long et les performances sont dégradées pendant ce temps.  
- **Utilisation** : Serveurs de fichiers, bases de données où un bon équilibre entre vitesse et sécurité est nécessaire.  
- **Nombre minimum de disques 💾** : 3  

---

### **4. RAID 6 (Double parité - Dual Parity)** 🏗️
- **Principe** : Similaire au RAID 5, mais avec **deux blocs de parité** pour offrir une protection contre la perte de **deux disques simultanément**.  
- ✅ **Avantages** :  
  ✔️ **Haute sécurité** : Protection contre la panne de deux disques en même temps.  
  ✔️ **Lecture rapide** : Les performances de lecture sont élevées.  
- ❌ **Inconvénients** :  
  ⚠️ **Écriture plus lente** : Le calcul de deux parités ralentit l'écriture.  
  ⚠️ **Capacité réduite** : La capacité totale est la somme des disques moins deux.  
- **Utilisation** : Environnements critiques nécessitant une haute disponibilité, comme les serveurs de données stratégiques.  
- **Nombre minimum de disques 💾** : 4  

---

### **5. RAID 10 (ou RAID 1+0)** 🔄
- **Principe** : Combinaison de **RAID 1 (miroir)** et **RAID 0 (entrelacement)**.  
  - Les données sont **miroitées** pour la redondance (RAID 1) puis **entrelacées** pour les performances (RAID 0).  
- ✅ **Avantages** :  
  ✔️ **Haute performance et sécurité** : Lecture et écriture rapides avec redondance totale.  
  ✔️ **Reconstruction rapide** : La reconstruction des données est rapide en cas de panne de disque.  
- ❌ **Inconvénients** :  
  ⚠️ **Capacité réduite** : Seule la moitié de la capacité totale est disponible (car les données sont dupliquées).  
  ⚠️ **Coût élevé** : Nécessite un grand nombre de disques.  
- **Utilisation** : Bases de données à haute performance, applications critiques nécessitant une vitesse et une redondance maximales.  
- **Nombre minimum de disques 💾** : 4 (2 pour le miroir et 2 pour l'entrelacement)  

---

### 📝 **Tableau récapitulatif des niveaux RAID**  

| **Niveau RAID 📊** | **Performances 🚀**         | **Redondance 🔄**              | **Capacité utile**           | **Nombre min. de disques 💾** | **Utilisation**                        |
|-----------------|--------------------------|------------------------------|------------------------------|-----------------------------|----------------------------------------|
| **RAID 0 ⚡**      | Très rapide               | Aucune                       | 100% de la somme des disques  | 2                           | Jeux, montage vidéo                     |
| **RAID 1 🔍**      | Lecture rapide, écriture normale | Redondance totale             | 50% de la somme des disques   | 2                           | Données critiques, bases de données     |
| **RAID 5 🛡️**      | Lecture rapide, écriture plus lente | Tolérance à 1 disque en panne | Somme des disques - 1        | 3                           | Serveurs de fichiers, stockage général  |
| **RAID 6 🏗️**      | Lecture rapide, écriture plus lente | Tolérance à 2 disques en panne| Somme des disques - 2        | 4                           | Environnements critiques                |
| **RAID 10 🔄**     | Très rapide               | Redondance totale             | 50% de la somme des disques   | 4                           | Bases de données haute performance      |

---

### 🎯 **En résumé**  
- Le **RAID** est utilisé pour améliorer les performances, la capacité de stockage et la sécurité des données.  
- **RAID 0 ⚡** pour la performance (pas de sécurité).  
- **RAID 1 🔍** pour la redondance maximale (copie exacte des données).  
- **RAID 5 🛡️** pour un bon compromis entre vitesse et sécurité.  
- **RAID 6 🏗️** pour une tolérance élevée aux pannes.  
- **RAID 10 🔄** pour les performances et la redondance maximales, mais à un coût élevé en disques.

---
- [Le Laboratoire 🔬](/Docs.md)

### 🛠️ **Montage Hardware**

Texte du chapitre ici...

### 🖥️ **Montage Software**

Texte du chapitre ici...

### 🐧 **Depuis Debian 12**

Texte du chapitre ici...

### 🏗️ **Depuis Proxmox**

Texte du chapitre ici...

### 🪟 **Depuis Windows Serveur**

Texte du chapitre ici...