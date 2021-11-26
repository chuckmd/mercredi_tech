# Guide moniteurs v2

*****


## Quelle taille (et définition) choisir ?

En français courant on utilise souvent le terme "résolution" pour parler du nombre de pixels affichés à l'écran, mais on parle en fait de "définition" (en anglais : resolution, d'où l'erreur). Une résolution prends en compte la taille de l'écran. Exemple :

* *1920 pixels horizontaux par 1080 pixels verticaux est une [définition](https://fr.wikipedia.org/wiki/D%C3%A9finition_d%27%C3%A9cran) (1920x1080/Full HD)*

* *1920x1080 à 24" est une [résolution](https://fr.wikipedia.org/wiki/R%C3%A9solution_spatiale_des_images_matricielles) (92 pixels par inch ou ppi)*

La principale caractéristiques d'un moniteur, c'est le nombre de pixels qu'il affiche. Et surtout à quel point on va pouvoir les distinguer.

Tout ça c'est [standardisé évidemment](https://en.wikipedia.org/wiki/Graphics_display_resolution), voici les plus communes :


| 16:9                 | Ultrawide (21:9)      |
| -------------------- | --------------------- |
| 1920 x 1080 (FHD)    | 2560 x 1080 (UW-FHD)  |
| 2560 x 1440 (QHD)    | 3440 x 1440 (UW-QHD)  |
| 3840 x 2160 (4K UHD) | 5120 x 2160 (UW-UHD)  |

Evidemment pour les joueurs, **plus la définition est élevée, plus la carte graphique doit travailler.** L'incrément n'est pas linéaire car les développeurs ont optimisé les drivers et les jeux, mais faire tourner un jeu en QHD ou en 4K sera nettement plus lourd qu'en FHD (mais sans solliciter plus le CPU).

> **Trigger warning sur la définition 2K :** ça ne veut rien dire, arrêtez de dire 2K pour dire QHD, c'est [une définition pour le mastering cinéma](https://videocide.com/glossary/dci-2k/) proche du FHD. Même les vendeurs s'y mettent maintenant, donc je me sens obligé de dire que ça signifie souvent **QHD**, mais c'est une erreur.




## Résolution (=définition/taille)

Ce qui est important donc, c'est **la résolution**, le rapport entre la **taille de l'écran** et sa **définition** (en ppi, pixel par inch). De mon expérience, on ne distingue plus les pixels à partir d'un taux d'environ 100 ppi. A l'inverse, un taux de ppi trop élevé va rendre les éléments illisibles.

Ca varie selon les gens et des dalles, ça dépends de facteurs différent comme votre acuité visuelle, le type de dalle, la distance oeil-écran, l'habitude ou tout simplement l'utilisation que vous faites de votre écran (un graphiste sera plus exigeant qu'un gamer sur ce point).

En partant de ce postulat, on peut définir **les résolutions idéales pour un écran confortable :**

* 24" : 1920x1080 -> 91 ppi

* 27" : 2560x1440 -> 108 ppi

* 32" : 3840x2160 -> 129 ppi

L'augmentation de la définition permet également de profiter de plus de superficie sur son bureau pour afficher des fenêtes, ce qu'on appelle le *real estate*. Comparaison du nombre de fenêtres qu'on peut afficher sur ces 3 définitions : [FHD](https://imgur.com/3lxAmGi), [QHD](https://imgur.com/cBNLWFJ), [4K](https://imgur.com/1kH7ONC). 

Pour la productivité, c'est génial car vous pourrez afficher plus d'éléments sur l'écran. Pour le gaming, l'image affichée aura toujours la même taille, c'est surtout une augmentation des détails (même si certains jeux permettent d'ajuster la taille de l'interface)

**Le scaling/HiDPI/Retina**

Les définitions trop élevées, si on laisse l'affichage en 100% natif, rendent le texte et les éléments [trop petits](https://www.memesmonkey.com/images/memesmonkey/08/084f157e54694987ecb05a49eee33e86.jpeg) pour les lire correctement. Heureusement, on peut changer la mise à l'échelle (scaling) : x1.25, 1.50, 1.75, 2.00... L'idéal étant un facteur entier de x2 (HiDPI/Retina), car [doubler les pixels se fait proprement](https://medium.com/elementaryos/what-is-hidpi-and-why-does-it-matter-b024eabea20d) (4 pixels = 1 pixel HiDPI), alors qu'avec un facteur fractionnel va utiliser des algorithmes d'anti-aliasing pour tricher.

Certaines applications peuvent être incompatibles avec le HiDPI et ne pas se mettre à l'échelle (ou être floues), même si ça devient rare. **Attention aussi si vous faites du multi-écran avec et sans HiDPI**, c'est potentiellement foireux.


*****


## Technologies de dalle

Je vous fais grâce de la science, j'en reparlerai pour ceux que ça intéresse. Retenez que c'est des **grilles de cellules à cristaux liquides** (LCD) à [matrices actives](https://en.wikipedia.org/wiki/Liquid-crystal_display#Active-matrix_technologies) avec différentes façon d'activer chaque cellule (envoyer une tension) et de les rétro-éclairer.

* **TN :** (Twisted Nematic) : très populaire du temps où on n'arrivait pas à faire des dalles haute fréquence avec les autres technos, c'est maintenant une technologie obsolète qui a de gros défauts (faibles angles de visions, couleurs exécrables). A oublier pour tout nouvel achat.

* **VA :** (Vertical Alingment) : des dalles qui brillent par leur contraste (enfin, je me comprends), mais pèchent sur les temps de réponse, induisant souvent du ghosting à haute fréquence. Les angles de vision et la fidélité colorimétrique sont également limités. Utile surtout si vous jouez à des jeux immersifs dans des environnements sombre (horreur, thriller...).

* **IPS :** (In-Plane Switching) : les meilleures sur la fidélité colorimétrique, les temps de réponse et les angles de vision. Elles ont cependant un contraste inférieur aux dalles VA, et sont plus sujettes aux fuites de lumière (backlight bleed). Pour jouer et travailler, c'est le meilleur des deux mondes.

* **OLED :** (Organic Light-Emitting Diode) : contrairement aux autres dalles qui utilisent des cristaux liquides (LCD), une dalle OLED est une grille de diodes microscopiques qui émettent leur propre lumière. Pour l'instant restreinte aux TV haut de gamme, smartphones et certains laptops ou écrans hors de prix, la technologie OLED est onéreuse mais promet de nombreux avantages : noirs parfaits, basse conso, pas de fuite de lumière... On espère juste que les problèmes de [burn-in](https://www.youtube.com/watch?v=hWrFEU_605g) seront réglés.


Il y a d'autres technos (PLS, AHVA...) mais c'est soit assez rare, soit une variante d'une des 4 technos principales.

**Tableau récapitulatif :**

| **Dalle** | **Taux de contraste** | **Rendu des couleurs** | **Rapidité**                    | **Angles de vision** | **Prix**  |
|-----------|------------|-------------|----------------|------------|-----------|
| TN        | Moyen      | Moyen       | Excellent      | Mauvais    | Abordable |
| VA        | Bon        | Bon         | Moyen/bon      | Moyen      | Abordable |
| IPS       | Moyen      | Bon         | Excellent      | Excellent  | Elevé      |
| OLED      | Excellent  | Excellent   | Excellent      | Excellent  | Abusif    |


> Note sur les dalles incurvées : en ultrawide (21:9), la courbe est là pour mieux épouser la vision en arc de l'oeil humain. **En 16:9 par contre, la courbe ne procure aucun avantage, elle existe pour réduire un défaut des dalles VA : les couleurs deviennent ternes sur les côtés.**


## Performance

Ce que j'ai résumé sous le terme "rapidité" ou "performance" jusqu'ici : les paramètres à prendre en compte pour du gaming :

* **Fréquence de rafraichissement (en Hertz) :** le nombre de fois que l'image peut être actualisée en une seconde. 60-75Hz pour de la bureautique, 120-170Hz pour du gaming, éventuellement 240Hz+ pour le gaming compétitif. 

* **Temps de réponse (en ms, mais rarement précisé) :** le temps qu'il faut pour qu'[un pixel change complètement de couleur](https://www.rtings.com/monitor/tests/motion/motion-blur-and-response-time). Le marketing utilise parfois le chiffre un peu menteur de 1ms, alors que le vrai temps de réponse moyen est plus proche des 6 ms sur un très bon écran.

* **Input lag (en ms) :** le délai entre l'action que vous effectuez et son affichage à l'écran. [Plus d'infos ici](https://www.rtings.com/monitor/tests/inputs/input-lag).

* **AdaptiveSync :** permet d'adapter la fréquence de rafraichissement aux fps que peut générer la carte graphique. Auparavant il fallait choisir entre Freesync (AMD, Intel) et G-Sync (Nvidia), maintenant la grande majorité des écrans récents sont Freesync + compatibles G-Sync.


Pour des performances optimales en jeu, on recherche évidemment l'écran avec la plus haute fréquence de rafraichissement et le plus bas input lag & temps de réponse possible. 

En pratique, la différence entre 60 et 144Hz est assez impressionnante (surtout si on revient à 60Hz après, c'est saccadé !). La différence entre 144Hz et 240Hz, en comparaison, n'est pas énorme, et même certains joueurs compétitifs se trompent en blind-test. Si votre budget est serré, privilégiez donc le 144Hz et un plus grand écran plutôt qu'un écran 24" 240Hz. 

Au delà de 240Hz, la différence est minime et même les plus exigeants des gamers privilégient les temps de réponse et d'autres critères plutôt qu'un écran 360Hz.

[Comparaison de fréquence filmée en slow motion](https://www.youtube.com/watch?v=Q1cmhZs1P54).




## Couleurs

Ici, le RGB ce n'est pas des bandes de LED sur l'écran, mais la fidélité colorimétrique, critère essentiel pour les professionnels de l'image et de la vidéo. 

* **Espaces colorimétriques :** on mesure en "pourcentage de couverture" la capacité d'un écran à afficher correctement une plage de couleur. Il en existe plusieurs : **sRGB** ou **Adobe RGB** pour la photo, **REC 709** ou **DCI-P3** pour la vidéo. La grande majorité des écrans IPS récents ont une excellente couverture du sRGB, mais pas forcément des autres espaces. [Explications](https://www.rtings.com/monitor/tests/picture-quality/color-gamut).
  
* **Calibrer sa dalle :** même les dalles d'excellente qualité nécessitent un calibrage pour être les plus fidèles possibles. Pour ceci, utilisez [une sonde de calibration](https://www.creativebloq.com/features/best-monitor-calibrator) et son logiciel associé. Aux dires des professionnels, il faut répéter l'opération tout les 2-3 mois. Le coût élevé de la sonde la réserve aux professionnels exigeants et aux entreprises.

* **La HDR (High Dynamic Range) :** on utilise une plage de couleurs plus importante (codée sur 8 ou 10 bits, au lieu de 6 bits), ce qui donne une image aux couleurs plus vives. Malheureusement la plupart des moniteurs actuels utilisent de la "fausse" HDR (HDR 400 : l'écran est compatible avec un signal HDR, mais en pratique la dalle ne permet pas de l'afficher proprement). Seuls quelques chers écrans 4K avec **local dimming** permettent d'afficher de la HDR digne de ce nom, dommage.

## Défauts potentiels des écrans

Malgré l'évolution des technologies de dalles, il reste des défauts présents sur les dalles LCD haute fréquence qu'on peine encore à corriger. Certaines dépendent un peu d'une "lotterie de la dalle", donc je n'ai pas de conseils pour les éviter, mais sachez que ça existe, et que si vous tombez dessus vous pouvez utiliser votre droit de rétractation (mais pas forcément la garantie) :

* **[Backlight bleed](https://www.displayninja.com/what-is-backlight-bleed/)** : fuites de lumières sur les bordures de l'écran, souvent signe d'un mauvais contrôle qualité. Exemple entre un [bon](https://imgur.com/a/WDHHL1r) et un [très mauvais](https://imgur.com/a/n8Merv3) élève (deux écrans que j'ai possédé).

* **[IPS glow](https://www.limscave.com/reduce-ips-glow)** : couleurs diffuses aux coins de l'écran, qui varient avec l'angle de vision (contrairement au backlight bleed). Beaucoup moins gênant que ce dernier, mais également signe d'un mauvais contrôle qualité.

* **[Ghosting/black smearing :](https://www.youtube.com/watch?v=D6g85vqdK2A)** une trace sombre laissée par les objets en mouvement, causée par un temps de transition trop élevé entre des couleurs sombres (temps de réponse). Typiquement présent sur les dalles VA.

* **[Overshoot :](https://blurbusters.com/faq/lcd-overdrive-artifacts/)** une couronne claire laissée par des objets en mouvement, causée par une exagération des corrections anti-ghosting (overdrive).


*******

# Quel écran acheter ?

Etoile = meilleur rapport qualité/prix de sa catégorie.

## C'est pas la taille qui compte (Entrée de gamme jeu/bureautique, 24" FHD IPS)

A petit budget, si vous privilégiez la performance à la taille. Faire des dalles performantes à cette taille c'est un procédé maitrisé, donc la plupart des écrans IPS à 200€ se valent et cette gamme a peu évolué ces dernières années. J'ai donc fait une sélection basée sur les fonctionnalités et l'ergonomie.

* **Dell S2421HS** (75Hz)- [150€](https://www.dell.com/fr-fr/shop/%C3%A9cran-dell-24-pouces-s2421hs/apd/210-axkq/moniteurs-et-accessoires-de-moniteur) - [review](https://www.youtube.com/watch?v=26uXBJeZ4PI) - Un moniteur pour de la bureautique ou du multimédia, fiable à petit prix. Le pied réglable est une fonctionnalité qui devrait être présente sur tout les moniteurs en entreprise.

* **ViewSonic XG2405** - [200€](https://fr.pcpartpicker.com/product/G9LwrH/viewsonic-xg2405-238-1920x1080-144-hz-monitor-xg2405) - [review](https://www.techporn.ph/review-viewsonic-xg2405-gaming-monitor/) - Un look qui ne plaira pas à tout le monde, mais tout les ajustements ergonomiques dont vous pouvez avoir besoin, et des performances excellentes.

* **AOC 24G2(U)** - [200€](https://fr.pcpartpicker.com/product/PbpmP6/aoc-24g2ubk-240-1920x1080-144-hz-monitor-24g2ubk) - [review 2](https://pcmonitors.info/reviews/aoc-24g2u-24g2/) - Comme le XG2405, excellent rapport qualité/prix. Pour avoir vu les deux je dirais que le AOC a un meilleur contraste, mais a un peu plus d'IPS glow (même si c'est un peu la lotterie).

Eventuellement intéressants en promo dans les 200-220€ : **[BenQ EX2510]((https://www.youtube.com/watch?v=vByC1RfUJSo))**, 


## Le sweet spot (jeu & création, 27"-32" QHD IPS)

Le sweet spot pour les gamers et créatifs exigeants. Au départ limités à 144Hz, ces écrans tendent de plus en plus vers les 170-180Hz au fur et à mesure que les technologies de fabrication de dalles évoluent.

* **Gigabyte M27Q** - [350€](https://fr.pcpartpicker.com/product/k8GnTW/gigabyte-m27q-270-2560x1440-170-hz-monitor-m27q) - [review](https://www.rtings.com/monitor/reviews/gigabyte/m27q) - Bien qu'il utilise un array de pixels BGR (pouvant affecter la clarté du texte), c'est un bon moniteur à prix serré. Dalle 170Hz performante, port USB Type-C et la killer feature : un switch KVM intégré ! Existe aussi en 32" (M32Q).

* **Dell S2721DGFA** - [360€](https://www.dell.com/fr-fr/shop/%C3%A9cran-de-gaming-dell-27-s2721dgfa/apd/210-axrq/moniteurs-et-accessoires-de-moniteur) - [review](https://www.rtings.com/monitor/reviews/dell/s2721dgf) - le meilleur moniteur de Dell, dalle LG overclockée à 165Hz et excellente qualité de fabrication. C'est le moniteur que j'ai acheté pour mon PC gaming, j'en suis très content ! **Meilleur rapport qualité/prix de sa catégorie**.

* **LG 27GP850-B** - [450€](https://fr.pcpartpicker.com/product/WWcG3C/lg-27gp850-b-270-2560x1440-165-hz-monitor-27gp850-b) - [review 1](https://www.rtings.com/monitor/reviews/lg/27gp850-b) ; [review 2] - Le nouveau flagship de LG, dont les dalles nano-IPS équipent une grande partie de cette sélection. Quelques petits avantages qui le placent au dessus du marché : le Black Frame Insertion, l'overclock à 180Hz et le support du DCI-P3 à 98%. A vous de voir si ça vaut la différence de prix. Existe en 32" (32GP850).

* **MSI MAG274QRF-QD** - [500€](https://www.materiel.net/produit/202007270084.html) - [review](https://www.youtube.com/watch?v=i3X3yFh0-gE) - Avec une dalle d'AU Optronics qui rivalise en performance avec les nano-IPS de LG en proposant un contraste supérieur. Mais son prix reste assez élevé.


## Push it to the limit (jeu compétitif, 24"-27" 240Hz)

Les nouveaux moniteurs IPS QHD 240Hz sont encore très chers et peinent à justifier leur prix, donc je vous recommande plus de rester sur du 24" 240Hz (si la fréquence c'est vraiment important pour vous, pour l'e-sport) ou du 27" 144-180Hz (le reste des joueurs).

* **Samsung Odyssey G7** - [650€](https://fr.pcpartpicker.com/product/L6zFf7/samsung-odyssey-g7-270-2560x1440-240-hz-monitor-lc27g75tqsuxen) - [review](https://www.rtings.com/monitor/reviews/samsung/odyssey-g7) : basiquement le seul écran VA qui rivalise avec les IPS sur la colorimétrie et la performance. Son contraste le rends également idéal pour les jeux sombres ou immersifs. Seul véritable soucis : la courbe des dalles VA, qui peut gêner surtout pour les utilisations créatives (distortion...). Existe en 27" ou 32". **Meilleur rapport qualité/prix de sa catégorie.**

* **Dell Alienware AW2721D** - [750€](https://www.dell.com/fr-fr/shop/%C3%A9cran-de-gaming-alienware-27-aw2721d/apd/210-axnu/moniteurs-et-accessoires-de-moniteur) - [review 1](https://www.rtings.com/monitor/reviews/dell/alienware-aw2721d) ; [review 2](https://www.youtube.com/watch?v=ZH3-ep-SNNk) - Difficile à recommander car le Samsung G7 est moins cher et plus polyvalent. Éventuellement si vous voulez à la fois du 240Hz et des grands angles de vision, au détriment du contraste.

* **Gigabyte AORUS FI27Q-X** - [750€] - [review 1](https://www.rtings.com/monitor/reviews/gigabyte/aorus-fi27q-x) ; [review 2](https://www.youtube.com/watch?v=CHXsV7YBCPE) - Il peine à se démarquer face au G7 ou à l'AW2721D, mais 



## Création professionnelle (1440p/4K 60Hz, couleurs fidèles)

Notez que les écrans IPS "gaming" cités précédemment peuvent très bien contenir à des créatifs, vérifiez la fidélité des couleurs mais la plupart supportent au moins le sRGB. Le meilleur des deux mondes, je vous dis.

Les programmeurs (à haut budget) peuvent être intéressés par des écrans 4K pour la netteté du texte. Même si ça sera difficile à justifier à son patron.

* **LG 27UL650-W** - [300€](https://fr.pcpartpicker.com/product/DDJmP6/lg-27ul650-w-270-3840x2160-60-hz-monitor-27ul650-w) - [review](https://www.rtings.com/monitor/reviews/lg/27uk650-w) - Un moniteur qui accuse un peu son âge et peut devenir difficile à trouver, mais qui offre la 4K à prix plancher. Son remplacant (UL850-W) peut être une bonne alternative sur une promo.

* **Dell S2721QS** - [360€](https://www.dell.com/fr-fr/shop/%C3%A9cran-dell-27-pouces-uhd-4k-s2721qs/apd/210-axky/moniteurs-et-accessoires-de-moniteur) - [review](https://www.rtings.com/monitor/reviews/dell/s2721qs) - Dell propose un moniteur 4K haute fidélité à un prix serré, qui rends basiquement obsolète toute sa gamme Ultrasharp (significativement plus chère) tant il est bon. Existe en 32" (S3221QS) mais c'est un VA. **Meilleur rapport qualité/prix de sa catégorie.**

* **ASUS ProArt Display PA278CV** - [450€](https://fr.pcpartpicker.com/product/MYTp99/asus-proart-display-pa278cv-270-2560x1440-75-hz-monitor-pa278cv) - [review](https://www.rtings.com/monitor/reviews/asus/proart-display-pa278cv) - Successeur du PA278QV. Globalement des couleurs aussi fidèles que le S2721QS, la 4K en moins. Surtout utile pour le port USB-C intégré, pouvant charger et servir de dock pour un PC portable.


## Ultrawide mon amour (34-38" 21:9)

Parfait pour la productivité, mais pour du gaming la compatibilité 21:9 dépendra beaucoup des jeux auquels vous jouez : ça variera de la simple déformation d'image ou crop "propre" sur les jeux récents (pour ne pas donner un avantage en multi), à des barres noires sur les bords droits et gauche, et dans le pire des cas des jeux plus anciens qui ne tournent tout simplement pas en 21:9 et seront déformés.


* **Dell S3422DWG** - 


*****

**Sources :**

[Sven.de - Calculateur de résolution (PPI)](https://www.sven.de/dpi/)

[UFO Test (ghosting/rafraichissement)](https://www.testufo.com/ghosting)

[Viewsonic - Monitor resolution and aspect ratio](https://www.viewsonic.com/library/tech/monitor-resolution-aspect-ratio/)

[Eizo - Pixel density 4K](https://www.eizo.com/library/basics/pixel_density_4k/)

[Hardware Unboxed - Explication et comparaison des 3 principales technos](https://www.youtube.com/watch?v=luLS-I9lubg)

[Why your HDR monitor is probably not HDR at all](https://www.tftcentral.co.uk/blog/why-your-hdr-monitor-is-probably-not-hdr-at-all-and-why-displayhdr-400-needs-to-go/)

*****

**Autres guides d'achat :**

[Rtings - Best gaming monitors under $300](https://www.rtings.com/monitor/reviews/best/gaming-monitors-under-300)

[Rtings - Best 1440p monitors](https://www.rtings.com/monitor/reviews/best/1440p-gaming-monitors)

[Rtings - Best Monitors For Photo Editing And Video Editing](https://www.rtings.com/monitor/reviews/best/by-usage/photo-editing-graphic-design)

[Hardware Unboxed - Best gaming monitors of 2021](https://www.youtube.com/watch?v=CEqQi6Ljq8g)

[TFTCentral selector](https://www.tftcentral.co.uk/selector.htm)

[Tableau non exhaustif des IPS 27" 144Hz](https://docs.google.com/spreadsheets/d/1Qpmp7R_Pk852TnObn-jn0r_J-ZyYdgMc48hco1DiiE0/edit#gid=0) relayé par /u/A_Neaunimes

[Monitor Hunter's fact sheet](https://docs.google.com/document/d/1illeNLsUfZ4KuJ9cIWKwTDUEXUVpplhUYHAiom-FaDo)


*****

Notes sur le guide :

* Pas ou peu d'écrans VA car 1) on commence à avoir des écrans IPS à prix similaire 2) les temps de réponse de la plupart des VA (et le ghosting/overshoot qui en résultent) les rendent moins intéressants pour le gaming. Eventuellement si vous voulez un excellent contraste au détriment des performances générales.

* Pas d'écran 4K 144Hz. Ca existe, mais je trouve que même en 2021 c'est un mauvais investissement car c'est encore très cher et qu'aucun GPU n'est capable de faire tourner les jeux récents en 4K 144Hz. J'ai eu de mauvaises expériences avec le local dimming également, techno encore inégale.

* Les catégories reflètent mon état d'esprit sur le marché des moniteurs, les omissions de ces gammes sont donc volontaires, mais les différents guides que j'ai mis en lien vous permettront de combler les trous si besoin.

* Pour les possesseurs de PlayStation 5 qui voudraient un écran pour jouer sur leur bureau, méfiez-vous : les PS5 n'acceptent que des résolutions FHD ou 4K. **Il existe cependant des écrans capables de downscaler la 4K en QHD**, ce qui vous permet de jouer sur un 27" sans vous ruiner. Ils sont mentionnés dans la "Monitor Hunter's fact sheet" (*console ready*).