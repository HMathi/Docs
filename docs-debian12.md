![body](https://banzaihobby.com/cdn/shop/files/Aoshima_Initial_D_Takumi_Fujiwara_AE86_Trueno_Project_D_Specification_-_BanzaiHobby-254450.jpg?v=1717061182&width=1100)

# **Debian 12**

- [Le Laboratoire](./Docs.md)

>Pour une bonne install et une connexions présente, prendre la netinst sinon DVD en hors réseaux mais il y aura quelque petit problème de paquet.

**Debian GNU/Linux installer menu (BIOS mode)**    
1. Aller dans `Advanced options`
2. Choisir `Graphical expert install`
3. Suivre les étapes suivante ⬇️

---

> **Etape 1** : Choix de la langue du système   
![1](./CC/Debian12/debian-installer_main-menu_0.png)
![2](./CC/Debian12/localechooser_languagelist_0.png)
![3](./CC/Debian12/localechooser_shortlist_0.png)
![4](./CC/Debian12/localechooser_preferred-locale_0.png)    
> **⚠️ Pas de case à cocher sur cette page**    
![5](./CC/Debian12/localechooser_supported-locales_0.png)

---

> **Etape 2** : Choix de la langue du clavier   
![6](./CC/Debian12/debian-installer_main-menu_1.png)
![7](./CC/Debian12/keyboard-configuration_xkb-keymap_0.png)

---

> **Etape 3** : Détection du support d'installation       
![8](./CC/Debian12/debian-installer_main-menu_2.png)
*(généralement la clé bootable utilisée)*    
![9](./CC/Debian12/hw-detect_select_modules_0.png)
![10](./CC/Debian12/cdrom-detect_success_0.png)

---

> **Etape 4** : Choix de composant supplémentaire à l'installation   
![11](./CC/Debian12/debian-installer_main-menu_3.png)    
> **⚠️ Pas de case à cocher sur cette page *(sauf si vous avez envie de rajouter des composants que vous connaissez)***    
![12](./CC/Debian12/anna_choose_modules_0.png)

---

> **Etape 5** : Détection des composants réseaux de l'ordinateur *(aucune action nécessaire ormis `Entrer`)*   
![13](./CC/Debian12/debian-installer_main-menu_4.png)

---

> **Etape 6** : Connexion à Internet *(plutôt important pour la suite)*    
![14](./CC/Debian12/debian-installer_main-menu_5.png)
![15](./CC/Debian12/netcfg_use_autoconfig_0.png)
![16](./CC/Debian12/netcfg_link_wait_timeout_0.png)   
> *Bien entendu vous prenez le nom que vous voulez, celui présent ci-dessous est par default*   
![17](./CC/Debian12/netcfg_get_hostname_0.png)  
> *PC entreprise => mettre domaine présent / PC personnel => étape suivante*  
![18](./CC/Debian12/netcfg_get_domain_0.png)

---

> **Etape 7** : Création du/des utilisateurs    
![19](./CC/Debian12/debian-installer_main-menu_6.png)    
> **⚠️ Cocher non pour un poste perso *(sinon tu n'auras pas les autorisation root/administrateur sur ton compte)***    
![20](./CC/Debian12/passwd_root-login_0.png)    
> *Bien entendu vous prenez le nom que vous voulez, celui présent ci-dessous est pour l'exemple*   
![21](./CC/Debian12/passwd_username_0.png)
![22](./CC/Debian12/passwd_user-fullname_0.png)    
> *Même chose pour le mot de passe, c'est juste pour l'exemple*   
![23](./CC/Debian12/passwd_user-password_0.png)

---

> **Etape 8** : Configuration de l'horloge   
![24](./CC/Debian12/debian-installer_main-menu_7.png)    
> **⚠️ Bien sélectionner oui pour l'utilisation du protocole NTP *(cela vous permet d'avoir la même heure que toute les autres machines)***  
![25](./CC/Debian12/clock-setup_ntp_0.png)   
> **⚠️ Ici on ne touche a rien !!**    
![26](./CC/Debian12/clock-setup_ntp-server_0.png)
![27](./CC/Debian12/time_zone_0.png)

---

> **Etape 9** : Détection des disques de votre ordinateur *(aucune action nécessaire ormis `Entrer`)*    
![28](./CC/Debian12/debian-installer_main-menu_8.png)

---

> **Etape 10** : Création des partitions pour le **système**, la **mémoire swap** *(est un espace sur le disque dur ou SSD utilisé comme extension de la RAM lorsque cette dernière est pleine, permettant au système de continuer à fonctionner même avec des ressources limitées, bien que cela soit beaucoup plus lent que la RAM. Elle aide à éviter les plantages en cas de surcharge de mémoire.)* et **grub** *(menu de démarrage de linux. Installation à l'**étape 14**)*     
![29](./CC/Debian12/debian-installer_main-menu_9.png)    
> Aucune manipulation nécessaire, le système s'occupe de tout créé pour vous *(dans cette exemple on ne l'utilise pas donc on passe notre chemin)*    
![30](./CC/Debian12/partman-auto_init_automatically_partition_0.png)    
> **Similaire au précédent**, car c'est le système qui s'en charge, mais avec une petite nuance : **LVM**(pour **Logical Volume Manager**) permet d'agrandir le stockage si nécessaire, et ce **sans perdre la moindre donnée**. *(très utile lors de la création de machine virtuel)*    
![31](./CC/Debian12/partman-auto_init_automatically_partition_1.png)    
> Le titre étant plutôt explicite je vous propose de commencer les deux exemples présent ci-dessous. ⬇️   
![32](./CC/Debian12/partman-auto_init_automatically_partition_2.png)

> **Montage LVM**    
![33](./CC/Debian12/partman-auto_select_disk_0.png)      
> Pour simplifier la gestion, surtout pour les débutants, il est souvent recommandé d'utiliser une seule partition principale où tout est installé, y compris la swap, plutôt que de créer plusieurs partitions *(comme une partition séparée pour `/home` ou `/var`)*. Cela facilite les sauvegardes et la gestion de l'espace disque.      
Cependant, pour les utilisateurs plus avancés ou pour une meilleure organisation, il peut être utile de créer des partitions distinctes *(par exemple, pour les données personnelles avec `/home`)*, car cela permet de mieux contrôler l'espace et d'isoler certaines parties du système pour une gestion plus flexible.     
![34](./CC/Debian12/partman-auto_choose_recipe_1.png)
![35](./CC/Debian12/partman-lvm_confirm_0.png)  
> *Bien entendu vous prenez le nom que vous voulez, celui présent ci-dessous est par default*   
![36](./CC/Debian12/partman-auto-lvm_new_vg_name_0.png)  
> *Taille de la partitions au choix selon ce que vous souhaitez faire.*    
![37](./CC/Debian12/partman-auto-lvm_guided_size_0.png)
![38](./CC/Debian12/partman_confirm_nooverwrite_1.png)   
> Vous n'aurez pas forcément ce menu qui s'affichera mais voilà à quoi ressemble la création de partition avec LVM *(si vous souhaitez le voir il suffit de retourner dans `Partitionner les disques` et de séléctionner `Manuel` ce qui vous donnera un visuel du disque et des partitions comme ci-dessous)*    
![39](./CC/Debian12/partman_choose_partition_3.png)

> **Montage Manuel**    
![40](./CC/Debian12/partman_choose_partition_0.png)      
> *La création d'une table de partitions te permet une meilleure organisation et une gestion plus efficace de ton disque dur, tout en apportant des avantages en termes de sécurité, de performance et de flexibilité.*    
![41](./CC/Debian12/partman-partitioning_confirm_new_label_0.png)    
> *Le choix se porte sur **GPT** car il est plus moderne, offrant des fonctionnalités comme UEFI, ainsi qu'une meilleure fiabilité et flexibilité dans la gestion des partitions.*     
![42](./CC/Debian12/partman-partitioning_choose_label_0.png)
![43](./CC/Debian12/partman_choose_partition_1.png)
![44](./CC/Debian12/partman_free_space_0.png)      
> Pour simplifier la gestion, surtout pour les débutants, il est souvent recommandé d'utiliser une seule partition principale où tout est installé, y compris la swap, plutôt que de créer plusieurs partitions *(comme une partition séparée pour `/home` ou `/var`)*. Cela facilite les sauvegardes et la gestion de l'espace disque.      
Cependant, pour les utilisateurs plus avancés ou pour une meilleure organisation, il peut être utile de créer des partitions distinctes *(par exemple, pour les données personnelles avec `/home`)*, car cela permet de mieux contrôler l'espace et d'isoler certaines parties du système pour une gestion plus flexible.     
![45](./CC/Debian12/partman-auto_choose_recipe_0.png)
![46](./CC/Debian12/partman_choose_partition_2.png)
![47](./CC/Debian12/partman_confirm_nooverwrite_0.png)

---

> **Etape 11** : Installation du système de base/Noyaux     
![48](./CC/Debian12/debian-installer_main-menu_10.png)
![49](./CC/Debian12/base-installer_kernel_image_0.png)
![50](./CC/Debian12/base-installer_initramfs-tools_driver-policy_0.png)

---

> **Etape 12** : Configuration de l'outils de gestion des paquets *(c'est ici que l'accès a internet joue un rôle important car si pas internet certains menu vont manquer a l'appel)*    
![51](./CC/Debian12/debian-installer_main-menu_11.png)
![52](./CC/Debian12/apt-setup_cdrom_set-first_0.png)     
> **⚠️ Très important de dire oui au miroir sur le réseaux car c'est lui qui apporte le plus de paquet a votre système.**     
![53](./CC/Debian12/apt-setup_use_mirror_0.png)
![54](./CC/Debian12/mirror_protocol_0.png)
![55](./CC/Debian12/mirror_http_countries_0.png)
![56](./CC/Debian12/mirror_http_mirror_0.png)
![57](./CC/Debian12/mirror_http_proxy_0.png)
![58](./CC/Debian12/apt-setup_services-select_0.png)     
> *Les deux questions suivantes vous permettront d'utiliser des logiciels et microprogrammes non pris en charge nativement par Debian, mais qui fonctionnent tout de même.*      
![59](./CC/Debian12/apt-setup_non-free_0.png)
![60](./CC/Debian12/apt-setup_non-free-firmware_0.png)
![61](./CC/Debian12/apt-setup_enable-source-repositories_0.png)

---

> **Etape 13** : Installation et choix de l'environnement   
![62](./CC/Debian12/debian-installer_main-menu_12.png)
![63](./CC/Debian12/pkgsel_update-policy_0.png)    
> *Personnellement je n'accepte pas d'y participer mais vous avez totalement la possibilité de la faire*    
![64](./CC/Debian12/popularity-contest_participate_0.png)      
> Pour le choix de l'environnement ou de l'interface, je vous laisse le libre choix. Je vous conseille de lire les descriptions sous l'image pour faire un premier choix, et ensuite, l'expérience vous aidera à déterminer celui qui vous plaît vraiment.  
J'ai également coché le serveur SSH, car il vous permet de vous connecter à votre machine à distance si vous êtes sur le même réseau. *(**Attention**, la connexion SSH se fait par le biais d'une console ; vous n'aurez pas de visuel graphique, seulement des lignes de commande. Je vous conseille donc d'apprendre un peu le bash, ce qui vous aidera à naviguer dans la console.)*     
![65](./CC/Debian12/tasksel_first_0.png)     
### 1. **GNOME**
   - **Interface** : Moderne, minimaliste, avec un design épuré.
   - **Philosophie** : Favorise la simplicité et l'efficacité. Beaucoup de tâches sont automatisées pour éviter les configurations manuelles.
   - **Performance** : Utilise plus de ressources système que les autres environnements de bureau légers.
   - **Personnalisation** : Moins personnalisable par défaut, mais extensible via des extensions.
   - **Caractéristiques** : Offre une interface utilisateur consistante, avec des éléments comme le dock et le tableau de bord en haut. Utilise Wayland par défaut dans les versions récentes.
   - **Idéal pour** : Les utilisateurs qui veulent une expérience simple et cohérente.

### 2. **Xfce**
   - **Interface** : Traditionnelle avec un menu en bas, légère et rapide.
   - **Philosophie** : Conçu pour être rapide et économe en ressources, tout en restant facile à utiliser et personnalisable.
   - **Performance** : Très léger, ce qui le rend adapté aux machines plus anciennes ou avec peu de ressources.
   - **Personnalisation** : Très personnalisable avec de nombreuses options de configuration.
   - **Caractéristiques** : Interface simple, avec un gestionnaire de fenêtres classique et un tableau de bord.
   - **Idéal pour** : Les utilisateurs qui ont besoin d'un environnement léger et rapide sans sacrifier trop de fonctionnalités.

### 3. **KDE Plasma**
   - **Interface** : Très moderne et visuellement riche, avec des effets visuels avancés.
   - **Philosophie** : Offrir une expérience complète et personnalisable, avec beaucoup d'options de configuration.
   - **Performance** : Plus lourd que des environnements comme Xfce ou LXQt, mais toujours assez performant, surtout avec les versions récentes de Plasma qui ont amélioré l'efficacité.
   - **Personnalisation** : Extrêmement personnalisable à tous les niveaux, du fond d'écran aux interactions avec les fenêtres.
   - **Caractéristiques** : Basé sur Qt, il inclut une suite complète d'applications et de réglages.
   - **Idéal pour** : Les utilisateurs qui aiment personnaliser leur bureau et veulent une interface moderne et riche en fonctionnalités.

### 4. **Cinnamon**
   - **Interface** : Traditionnelle mais moderne, inspirée de GNOME 2, avec un menu de démarrage classique et des effets visuels.
   - **Philosophie** : Conçu pour être simple tout en offrant une expérience plus moderne que les environnements classiques.
   - **Performance** : Consomme plus de ressources que Xfce, mais reste assez léger comparé à GNOME ou KDE.
   - **Personnalisation** : Personnalisable avec des applets et des extensions, tout en restant accessible aux débutants.
   - **Caractéristiques** : Intègre de nombreux outils pour faciliter la gestion du bureau (par exemple, des applets de gestion de fenêtres, un système de menus configurable).
   - **Idéal pour** : Ceux qui recherchent un bureau traditionnel avec des fonctionnalités modernes et une interface élégante.

### 5. **MATE**
   - **Interface** : Traditionnelle, inspirée de GNOME 2, simple et sans fioritures.
   - **Philosophie** : Maintenir un bureau classique qui reste léger tout en étant fonctionnel.
   - **Performance** : Très léger et rapide, adapté aux systèmes plus anciens.
   - **Personnalisation** : Personnalisable, mais moins que KDE ou Cinnamon.
   - **Caractéristiques** : Utilise les technologies GTK+2 et GTK+3. Il conserve un aspect de bureau classique avec un gestionnaire de fenêtres et un tableau de bord traditionnel.
   - **Idéal pour** : Les utilisateurs qui préfèrent une interface simple et fonctionnelle, ou ceux qui souhaitent garder un environnement GNOME 2 classique.

### 6. **LXDE**
   - **Interface** : Très simple et minimaliste, avec une interface classique.
   - **Philosophie** : Conçu pour être léger, rapide et économe en ressources.
   - **Performance** : Très léger, adapté aux ordinateurs plus anciens ou avec peu de mémoire.
   - **Personnalisation** : Moins personnalisable que Xfce ou KDE, mais suffisamment pour la plupart des utilisateurs.
   - **Caractéristiques** : Moins d'effets visuels, mais une expérience utilisateur simple et rapide.
   - **Idéal pour** : Les utilisateurs qui cherchent un environnement extrêmement léger et rapide, particulièrement sur des machines avec des ressources limitées.

### 7. **LXQt**
   - **Interface** : Moderne et légère, similaire à LXDE mais plus moderne et avec des composants utilisant Qt.
   - **Philosophie** : Fournir une expérience légère et rapide avec une interface plus moderne que LXDE.
   - **Performance** : Léger et rapide, mais légèrement plus moderne que LXDE grâce à l'utilisation de Qt.
   - **Personnalisation** : Moins personnalisable que KDE ou Xfce, mais offre tout de même des options pour ajuster l'apparence.
   - **Caractéristiques** : Basé sur Qt, il utilise des composants modernes tout en restant très léger et rapide.
   - **Idéal pour** : Ceux qui veulent un bureau léger mais plus moderne que LXDE, avec un design basé sur Qt.

### Résumé des différences principales :
- **Légèreté** : Xfce, LXDE et LXQt sont les plus légers, parfaits pour les machines anciennes.
- **Personnalisation** : KDE Plasma est le plus personnalisable, suivi de près par GNOME et Cinnamon.
- **Design moderne** : GNOME, KDE Plasma et Cinnamon offrent des interfaces modernes et visuellement attrayantes.
- **Simplicité** : MATE et Cinnamon offrent une expérience plus classique et simple, tandis que GNOME est plus épuré.
- **Performance** : Xfce, LXDE et LXQt sont les plus performants sur des machines moins puissantes.

---

> **Etape 14** : Installation de GRUB     
![66](./CC/Debian12/debian-installer_main-menu_13.png)
![67](./CC/Debian12/grub-installer_only_debian_0.png)    
> Exécuter **os-prober** est utile si vous avez plusieurs systèmes d'exploitation sur votre ordinateur *(dual-boot)*.   
![68](./CC/Debian12/grub-installer_enable_os_prober_otheros_no_0.png)
![69](./CC/Debian12/grub-installer_choose_bootdev_0.png)

---

> **Etape 15** : Finalisation de l'installation    
![70](./CC/Debian12/debian-installer_main-menu_14.png)
![71](./CC/Debian12/clock-setup_utc_0.png)
![72](./CC/Debian12/finish-install_reboot_in_progress_0.png)

---
- [Le Laboratoire](./Docs.md)