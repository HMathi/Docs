![body](https://banzaihobby.com/cdn/shop/files/Aoshima_Initial_D_Takumi_Fujiwara_AE86_Trueno_Project_D_Specification_-_BanzaiHobby-254450.jpg?v=1717061182&width=1100)

# Qu'est-ce qu'un dual boot ?

- [Le Laboratoire](/Docs.md)

Le **dual boot** (ou double démarrage) est une configuration où deux systèmes d'exploitation différents sont installés sur un même ordinateur. Lors de l'allumage de l'ordinateur, tu choisis lequel des deux systèmes tu souhaites utiliser.

---

### Comment ça fonctionne ?

1. **Installation de plusieurs systèmes** :
   Un ordinateur avec dual boot a généralement deux systèmes d'exploitation installés sur des partitions séparées de son disque dur. Par exemple :
   - **Windows** sur une partition
   - **Linux** sur une autre partition

2. **Gestion du démarrage** :
   Quand tu allumes l'ordinateur, un **gestionnaire de démarrage** (aussi appelé **bootloader**) apparaît. Ce programme te permet de choisir le système d'exploitation à démarrer (Windows, Linux, etc.). Si tu ne choisis rien, le gestionnaire lance par défaut un des deux systèmes.

---

### Comment installer un **dual boot** ?

1. **Préparation de l'ordinateur** :
   - Si tu n’as pas encore installé les systèmes, commence par **installer Windows**. Windows aime être installé en premier sur la partition principale de l'ordinateur.
   - Pour installer Windows 10 ou 11, tu as à ta disposition les deux documentations suivantes :
   - [Windows 10](./docs-win10.md)
   - [Windows 11](./docs-win11.md)
   
2. **Création de partitions** :
   - Il faut créer deux partitions distinctes sur le disque dur : une pour Windows et une pour Linux. Linux peut redimensionner la partition Windows pendant son installation, ou tu peux le faire manuellement avant l'installation.
   - Voici les étapes à suivre pour modifier les partitions de disque sous Windows :

3. **Utilisation d'une clé bootable** :
   - Une fois les partitions créées, il te faut insérer ta clé bootable et redémarrer ton ordinateur. Durant le redémarrage, tu dois maintenir la touche `Échap` ou spammer la touche `F7` pour soit ouvrir le **BIOS** et indiquer à l'ordinateur de démarrer sur la clé, soit laisser l'ordinateur détecter tout seul la clé bootable et démarrer dessus.
   - Pour avoir une clé bootable, je te conseille ces trois documentations qui présentent différents logiciels de création de clés :
   - [Ventoy](/Outils/docs-ventoy.md)
   - [Rufus](/Outils/docs-rufus.md)
   - [Balena Etcher](/Outils/docs-balenaetcher.md)

4. **Installation de Linux** :
   - Une fois Windows installé, tu peux installer **Linux** sur la partition dédiée. Lors de l'installation, Linux détecte Windows et configure automatiquement le **bootloader** (souvent GRUB) pour te permettre de choisir le système au démarrage.
   - Pour installer Linux, tu as à ta disposition les deux documentations suivantes :
   - [Debian 12](./docs-debian12.md)
   - [Ubuntu](./docs-ubuntu.md)

5. **Choisir son système** :
   Après l'installation, au démarrage, tu verras un menu qui te permet de choisir entre Windows et Linux. Si tu ne fais pas de choix dans un certain délai, le système par défaut (souvent Windows ou Linux) se lancera automatiquement.

---

### Avantages du **dual boot** :

1. **Accès à deux systèmes d'exploitation** :
   - Tu peux utiliser des logiciels ou des jeux qui ne sont disponibles que sur un des systèmes. Par exemple, certains jeux ne fonctionnent que sous Windows, tandis que certains outils de développement sont optimisés pour Linux.

2. **Performances maximales** :
   - Contrairement aux **machines virtuelles** où le système d'exploitation tourne à l'intérieur d'un autre, le **dual boot** utilise toute la puissance de l'ordinateur pour chaque système. Cela permet de bénéficier de meilleures performances pour des tâches lourdes.

3. **Test d'un autre système sans risques** :
   - Tu peux essayer un nouveau système, comme Linux, tout en conservant Windows. Cela te permet de t'habituer à Linux sans abandonner Windows pour autant.

---

### Inconvénients du **dual boot** :

1. **Gestion de l'espace disque** :
   - Chaque système d'exploitation nécessite un espace dédié. Si tu n'as pas assez d'espace disque, tu pourrais rencontrer des problèmes de performance ou d’espace insuffisant pour tes fichiers.

2. **Redémarrage nécessaire** :
   - Pour passer d’un système à l’autre, il faut redémarrer l'ordinateur à chaque fois, ce qui peut être un peu contraignant par rapport à une machine virtuelle où tu peux basculer entre les systèmes sans redémarrer.

3. **Problèmes de mise à jour** :
   - Parfois, une mise à jour de Windows ou de Linux peut perturber le gestionnaire de démarrage, rendant difficile le choix du système. Heureusement, ce genre de problème peut généralement être réparé.

---

### Conclusion :

Un **dual boot** est une excellente solution si tu veux utiliser deux systèmes d'exploitation sur le même ordinateur. Que tu sois un passionné de technologie qui veut tester un autre OS, ou un utilisateur ayant des besoins spécifiques pour certains logiciels, le dual boot te permet de profiter des avantages de deux mondes différents.

Si tu souhaites garder Windows pour tes jeux et applications, mais utiliser Linux pour sa flexibilité et ses outils open source, alors le **dual boot** est fait pour toi !

---
- [Le Laboratoire](/Docs.md)