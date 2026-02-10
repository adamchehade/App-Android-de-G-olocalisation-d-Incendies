# App-Android-de-G-olocalisation-d-Incendies

# 🔥 FireLoc : Géolocalisation d'Incendies par Trigonométrie

**FireLoc** est une application Android innovante conçue pour les services de surveillance forestière et les citoyens vigilants. Elle permet de calculer les coordonnées GPS précises d'un départ de feu simplement en prenant une photo de la fumée, facilitant ainsi une intervention rapide des secours.

---

## 📸 Aperçu de l'Interface



*Capture d'écran montrant l'analyse de la fumée et le calcul des coordonnées en temps réel.*

---

## ✨ Fonctionnalités Clés

* **Calcul de Position Distante** : Utilise l'azimut (boussole), l'inclinaison de l'appareil et des algorithmes trigonométriques pour transformer un point visuel en coordonnées GPS ($Lat, Long$).
* **Alerte Automatique par SMS** : Dès que le calcul est validé, l'application génère et envoie automatiquement un SMS contenant la localisation précise du sinistre aux services d'urgence configurés.
* **Précision Terrain** : Intégration des données de capteurs internes (magnétomètre, accéléromètre) pour une mesure d'angle fiable.
* **Interface Réactive** : Flux caméra fluide avec interface de visée intuitive.

---

## 📐 Fonctionnement Technique

L'application repose sur la résolution de problèmes géométriques dans un espace 3D. Pour estimer la position du feu, le système utilise :

1.  **La position de l'observateur** ($A$) via le GPS du téléphone.
2.  **L'Azimut** ($\alpha$) : L'angle horizontal par rapport au Nord.
3.  **L'Angle d'inclinaison** ($\theta$) : Utilisé avec une estimation de la distance ou une triangulation par rapport à une base connue.




---

## 🚀 Installation & Configuration

1.  **Prérequis** : Un smartphone Android avec GPS, Boussole et Accéléromètre fonctionnels.
2.  **Permissions** :
    * `CAMERA` : Pour viser le départ de feu.
    * `ACCESS_FINE_LOCATION` : Pour connaître la position de l'utilisateur.
    * `SEND_SMS` : Pour l'envoi automatique de l'alerte.
3.  **Paramétrage** :
    * Ouvrez les réglages de l'application pour définir le numéro d'urgence par défaut (ex: 18 ou centre de secours local).

---

## 🛠️ Stack Technique

* **Langage** : Kotlin / Java (Android SDK)
* **Calculs** : Math library pour la trigonométrie sphérique.
* **Localisation** : Google Play Services Location API.
* **Communication** : SMS Manager API.

---

## 🤝 Contribution

Ce projet est ouvert aux contributions. Si vous souhaitez améliorer la précision des algorithmes (intégration de modèles de terrain MNT) ou l'interface utilisateur, n'hésitez pas à ouvrir une *Pull Request*.

---

### 👨‍💻 Développeur
* **Adam Chehade** - [GitHub](https://github.com/adamchehade)
