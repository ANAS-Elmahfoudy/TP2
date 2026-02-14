








<img width="365" height="784" alt="image" src="https://github.com/user-attachments/assets/2e3597a2-9b20-4d1d-9c64-7de735bf06d3" />
<img width="563" height="348" alt="image" src="https://github.com/user-attachments/assets/054cb6a9-81a4-4625-8bf3-a8a4d691cd4a" />
<img width="980" height="558" alt="image" src="https://github.com/user-attachments/assets/eb957cc8-8f7e-4809-bbff-0448a3a03b1b" />

















	



•  Scénario 1 : Exploration de l'interface principale
•	Action : Lancer l'application et naviguer sur l'écran d'accueil.
•	Objectif : Vérifier la stabilité de l'application sur un système rooté et identifier les menus disponibles.
•	Documentation : Capture d'écran de l'accueil avec identification de la version.
•  Scénario 2 : Recherche d'un élément ou d'un flag
•	Action : Utiliser la barre de recherche ou accéder à une catégorie spécifique (ex: "Search for a Flag").
•	Objectif : Simuler une interaction utilisateur standard pour observer le comportement des champs de saisie.
•	Documentation : Capture d'écran du texte saisi et du bouton cliqué.
•  Scénario 3 : Accès à une fiche de détail ou un challenge
•	Action : Ouvrir une fiche produit, un profil ou un challenge technique.
•	Objectif : Analyser le chargement des données et préparer l'interception des requêtes lors des étapes suivantes (Analyse dynamique).
•	Documentation : Capture d'écran du contenu affiché.

Etape 6
Voici la synthèse des piliers de la sécurité Android et l'impact du rooting :
•	Sandboxing des applications : Chaque application est isolée des autres dans son propre environnement sécurisé.
•	Modèle de permissions : Un système qui contrôle rigoureusement l'accès aux ressources sensibles comme la caméra ou les contacts.
•	Isolation et intégrité globale : Une protection native contre toute modification non autorisée du système de fichiers.
•	Impact du Root : Le rooting brise ces barrières de protection (sandboxing), permettant d'accéder à des zones normalement protégées et d'outrepasser les contrôles d'intégrité.

etape 7

 

etap 8

etap 9
-  Privilèges élevés : Le rooting consiste à obtenir les privilèges "super-utilisateur" (root) sur le système Android.
-  Modification des protections : Cette manipulation modifie les protections natives et la confiance globale du système de fichiers.
-  Utilité technique : C'est une étape indispensable en laboratoire pour observer certains comportements d'applications qui seraient invisibles autrement.
-  Gestion des risques : Bien que risqué, le rooting nécessite un isolement strict (réseau test), une traçabilité des actions et un reset complet après l'audit.


1. Définition du Rooting 
•	Définition : C'est l'obtention des privilèges "super-utilisateur" sur Android.
•	Impact : Cela modifie les protections natives et la confiance globale du système.
•	Usage : Indispensable en labo pour observer des comportements d'applications invisibles autrement.
•	Sécurité : Risqué, donc nécessite un isolement réseau, une traçabilité et un reset final.

2. Sécurité Android & Verified Boot 
•	Piliers de sécurité : Sandboxing (isolation), modèle de permissions, et intégrité globale.
•	Verified Boot : Garantit que le système démarré est celui du fabricant (Chain of Trust).
•	AVB (Android Verified Boot) : Version 2.0 plus moderne avec protection anti-rollback (empêche le retour à des versions vulnérables).
•	Commande Check : adb shell getprop ro.boot.verifiedbootstate (Attendu: Green).


3. Audit & Scénarios 
•	Périmètre : App (ex: InjuredAndroid), Support (AVD Pixel 6), Objectif (Rooting impact).
•	Installation : adb install app-debug.apk.
•	Scénarios de test : 1. Explorer l'accueil. 2. Rechercher un item/flag. 3. Ouvrir un détail (profil/fiche).



4. Standards OWASP MASVS 
•	STORAGE-1 : Les données sensibles doivent être chiffrées au stockage.
•	NETWORK-1 : Les communications doivent utiliser TLS avec des certificats valides.






