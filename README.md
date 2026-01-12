# Détecteur de Couleur – Arduino & Capteurs Optiques

## 📌 Description
Ce projet vise à concevoir un système embarqué capable de détecter des couleurs (rouge, vert, bleu, etc.) à l’aide d’un microcontrôleur Arduino, d’un capteur de couleur (TCS3200 / TCS34725) et d’un écran LCD.

Le système devait identifier une couleur et afficher son nom ainsi que son code (ex: #FF0000 pour le rouge).

Ce projet a été réalisé dans un cadre académique et met l’accent sur l’analyse, l’expérimentation et la compréhension des limites techniques.

---

## 🧠 Principe de fonctionnement
Le capteur de couleur mesure la lumière réfléchie par un objet.
Chaque couleur réfléchit différemment les longueurs d’onde (R, G, B).
L’Arduino lit les valeurs issues du capteur, les traite, puis détermine la couleur la plus probable.
Le résultat est affiché sur un écran LCD.

---

## 🧰 Composants utilisés
- Arduino Uno  
- Capteur de couleur TCS3200 / TCS34725  
- Écran LCD 16x2 ou 20x4  
- Potentiomètre  
- Résistances, câbles et breadboard  

---

## 🖥️ Logiciels
- Arduino IDE  
- Tinkercad Circuits (simulation)  
- Proteus ISIS (schéma & simulation)

---

## ⚠️ Problèmes rencontrés
Le projet a révélé plusieurs limites techniques importantes :

- Le capteur TCS3200 n’est pas disponible nativement dans Proteus
- Les modèles simulés donnent des sorties trop simplifiées (0/1 au lieu de valeurs analogiques réelles)
- La calibration des seuils de couleurs est très sensible à l’éclairage
- Les capteurs optiques sont fortement influencés par la lumière ambiante

Ces contraintes ont empêché une détection fiable dans l’environnement de simulation.

---

## 🔬 Approche alternative proposée
Pour dépasser ces limites, nous avons proposé un système basé sur un principe de spectrométrie :

- Utiliser plusieurs LEDs (R, G, B)
- Mesurer la lumière réfléchie via photodiodes ou photo-résistances
- Calculer le pourcentage de réflexion pour chaque couleur
- Déterminer la couleur dominante par traitement Arduino

Cette approche est plus réaliste, mais plus complexe à réaliser matériellement.

---

## 📄 Rapport
Le rapport complet du projet est disponible dans le dossier et contient :
- les schémas,
- la théorie,
- les tests,
- et l’analyse des limites du système.

---

## 🎯 Ce que j’ai appris
- Fonctionnement des capteurs optiques
- Interaction lumière-matière
- Difficultés de la simulation électronique
- Importance de la calibration
- Méthode d’analyse en ingénierie

---

## 👤 Auteurs
- Zoubai Douha  
- Mtahtah Wissal  

Encadrante : Madame Zakriti
