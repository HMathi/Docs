![body](https://banzaihobby.com/cdn/shop/files/Aoshima_Initial_D_Takumi_Fujiwara_AE86_Trueno_Project_D_Specification_-_BanzaiHobby-254450.jpg?v=1717061182&width=1100)

# 🔑 Ventoy

- [Le Laboratoire 🔬](/Docs.md)

📥 **Lien de téléchargement :**
- [Lien](https://www.ventoy.net/en/download.html) - site source
- [Lien](https://lecrabeinfo.net/telecharger/ventoy/) - version un peu ancienne

---

### 💡 **Qu'est-ce que Ventoy ?**

**Ventoy** est un outil gratuit et open-source qui permet de créer une clé USB bootable de manière simple et efficace. Contrairement aux outils classiques qui nécessitent de "graver" une image ISO sur une clé USB, **Ventoy** fonctionne différemment :  

- Tu installes **Ventoy** sur ta clé USB une seule fois.  
- Ensuite, tu peux simplement **copier-coller** des fichiers **ISO** sur la clé (Windows, Linux, outils de réparation, etc.).  
- Au démarrage, un menu te permet de **choisir l'ISO à lancer** sans avoir à reformater la clé à chaque fois.  

---

### 🔍 **Comment fonctionne Ventoy ?**

1. **Installation sur une clé USB** 📥 
   - Tu télécharges **Ventoy** depuis son site officiel.  
   - Tu lances l’outil et installes **Ventoy** sur ta clé USB (attention, cela efface les données de la clé lors de l'installation).  

2. **Ajout des fichiers ISO** 📀 
   - Une fois installé, **ta clé USB devient un simple espace de stockage**.  
   - Il te suffit de **copier-coller** tes fichiers ISO directement dessus (Windows, Linux, outils de dépannage, etc.).  

3. **Utilisation au démarrage** 🚀 
   - Branche la clé USB sur un PC et redémarre en accédant au menu de **boot** (souvent en appuyant sur **F2, F12, ESC ou DEL** selon l’ordinateur).  
   - **Ventoy** affiche un menu avec la liste des ISO présents sur la clé.  
   - Tu sélectionnes celui que tu veux et **l'ordinateur démarre dessus** comme si tu avais gravé l'ISO sur une clé classique.  

---

### 📊 **Comparaison avec d’autres outils**  

| Fonctionnalité        | Ventoy | Rufus | Etcher |
|----------------------|--------|-------|--------|
| **Formatage nécessaire** | ❌ Non | ✅ Oui | ✅ Oui |
| **Multi-ISO sur une clé** | ✅ Oui | ❌ Non | ❌ Non |
| **Vitesse d’écriture** | ⏳ Moyenne | 🚀 Très rapide | ⏳ Moyenne |
| **Compatibilité OS** | 🖥️ Windows/Linux | 🖥️ Windows uniquement | 🖥️ Windows/Linux/macOS |
| **Taille du logiciel** | 📦 ~30 Mo | 📦 ~1 Mo | 📦 ~120 Mo |
| **Supporte Windows et Linux** | ✅ Oui | ✅ Oui | ✅ Oui |

**Rufus** est plus rapide pour une **installation unique** d’un OS sur une clé, tandis que **Ventoy** est la meilleure solution si tu veux conserver **plusieurs ISO sur la même clé sans reformater**.  

---

### ✅ **Avantages de Ventoy**  

✔️ **Pas besoin de reformater la clé**  
   - Contrairement aux outils comme **Rufus** ou **UNetbootin**, où il faut créer une clé bootable à chaque fois, avec **Ventoy**, tu n’as qu’à glisser-déposer tes fichiers ISO !  

✔️ **Multi-ISO sur une seule clé**  
   - Tu peux stocker **plusieurs systèmes ou outils** sur une seule clé (Windows, Ubuntu, Kali Linux, outils de récupération, etc.).  
   - Plus besoin d’avoir plusieurs clés USB pour différents systèmes !  

✔️ **Compatible avec UEFI et Legacy BIOS**  
   - **Ventoy** fonctionne aussi bien sur les anciens ordinateurs en **mode BIOS** que sur les nouveaux en **mode UEFI**, ce qui le rend très flexible.  

✔️ **Mises à jour simples**  
   - Si un nouveau système sort, pas besoin de tout recommencer. Il suffit de **copier le nouvel ISO** sur la clé, et c’est tout !  

✔️ **Supporte plus de 1000 ISOs**  
   - Ventoy est compatible avec **une grande variété de fichiers ISO**, y compris les systèmes Windows, Linux, et les outils de réparation comme Hiren's BootCD ou Medicat.  

---

### ❌ **Inconvénients de Ventoy**  

⚠️ **Installation initiale obligatoire**  
   - Avant de l’utiliser, il faut **installer Ventoy sur la clé**, ce qui supprime toutes les données existantes sur celle-ci.  

⚠️ **Certains ISOs peuvent ne pas fonctionner**  
   - Bien que **Ventoy** supporte la plupart des fichiers ISO, certains peuvent avoir des problèmes de compatibilité (surtout les systèmes très personnalisés). Heureusement, **Ventoy est régulièrement mis à jour** pour améliorer cela.  

⚠️ **Dépendance au BIOS/UEFI**  
   - Certains PC anciens ou spécifiques peuvent ne pas reconnaître **Ventoy** correctement, surtout s'ils ont des paramètres BIOS restreints.  

---

### 🎯 **Alternative à Ventoy**  

Si tu veux un outil plus simple sans installation initiale, il existe des alternatives comme **Rufus**, **Etcher** ou **UNetbootin**, mais elles nécessitent de créer une nouvelle clé bootable pour chaque ISO. **Ventoy** reste le meilleur choix si tu veux gérer plusieurs ISOs sur une seule clé !  

---

### 📜 **Installation :**

> **Etape 1** : Unzip le fichier pour pouvoir lancer l'application.     
![](/CC/Ventoy/1.png)      
> **Etape 2** : Lancer `Ventoy2Disk.exe`.    
![](/CC/Ventoy/2.png)      
![](/CC/Ventoy/3.png)      
> **Etape 3** : Choisissez la clé qui vous servira à stocker et utiliser les différents ISO téléchargés.    
![](/CC/Ventoy/4.png)      
![](/CC/Ventoy/5.png)      
> **Etape 4** : Formatage de la clé avec un double check.      
![](/CC/Ventoy/6.png)      
![](/CC/Ventoy/7.png)      
> **Etape 5** : Lancement de l'installation.    
![](/CC/Ventoy/8.png)      
> **Etape 6** : C'est fini, votre clé est utilisable.    
![](/CC/Ventoy/9.png)      
> **Bonus** : Voici les paramètres et le choix de la langue.      
![](/CC/Ventoy/10.png)     
![](/CC/Ventoy/11.png)     
> *Voici à quoi ressemble votre clé suite à la manipulation.*     
![](/CC/Ventoy/12.png)     

---
- [Le Laboratoire 🔬](/Docs.md)