# Projet C++ : Système de Suivi et de Réduction des Déchets Alimentaires

## Contexte du projet
Le gaspillage alimentaire est un problème majeur à l'échelle mondiale, tant du point de vue environnemental qu'économique. Ce projet vise à développer une application en C++ permettant de suivre, d'analyser et de réduire les déchets alimentaires à domicile ou dans une petite structure (restaurant, cantine, etc.). L'application aidera les utilisateurs à enregistrer les aliments achetés, à surveiller leur consommation, et à identifier les aliments périmés pour réduire le gaspillage.

## Cahier des charges

### 1. Objectifs généraux
- Développer une application console en C++ pour la gestion et la réduction des déchets alimentaires.
- Permettre aux utilisateurs de suivre les produits alimentaires qu'ils achètent, consomment ou jettent.
- Fournir des statistiques sur les habitudes de consommation et des conseils pour réduire le gaspillage.
- Offrir des alertes pour les produits approchant de leur date de péremption.

### 2. Fonctionnalités principales

1. **Suivi des achats alimentaires :**
   - Enregistrement des produits alimentaires avec leur nom, quantité, date d'achat et date de péremption.
   - Mise à jour de l'inventaire lors de la consommation ou du jet des produits.

   **Exemple de sortie console :**
   ```
   --- Suivi des Achats Alimentaires ---

   Entrez le nom du produit : Lait
   Entrez la quantité (en litres) : 1
   Entrez la date d'achat (JJ/MM/AAAA) : 25/08/2024
   Entrez la date de péremption (JJ/MM/AAAA) : 30/08/2024

   Produit ajouté avec succès :
   Nom : Lait
   Quantité : 1 litre
   Date d'achat : 25/08/2024
   Date de péremption : 30/08/2024
   ```

2. **Suivi des produits :**
   - Affichage de l'inventaire des produits alimentaires.
   - Permettre à l'utilisateur de mettre à jour l'inventaire lorsqu'il consomme ou jette un produit.

   **Exemple de sortie console :**
   ```
   --- Inventaire des Produits Alimentaires ---

   Produit : Lait
   Quantité : 1 litre
   Date d'achat : 25/08/2024
   Date de péremption : 30/08/2024

   Que voulez-vous faire avec ce produit ?
   1. Consommer
   2. Jeter
   3. Rien

   Choix : 1
   Entrez la quantité consommée (en litres) : 0,5

   Inventaire mis à jour :
   Nom : Lait
   Quantité restante : 0,5 litre
   Date de péremption : 30/08/2024
   ```

3. **Alerte de péremption :**
   - Notifier l'utilisateur lorsqu'un produit approche de sa date de péremption pour éviter le gaspillage.

   **Exemple de sortie console :**
   ```
   --- Alerte de Péremption ---

   ATTENTION : Le produit suivant approche de sa date de péremption !

   Produit : Lait
   Quantité : 0,5 litre
   Date de péremption : 30/08/2024
   Consommez ce produit rapidement pour éviter le gaspillage.
   ```

4. **Analyse des habitudes et statistiques :**
   - Fournir des statistiques sur les habitudes alimentaires de l'utilisateur, comme la quantité de nourriture gaspillée, et donner des recommandations pour réduire le gaspillage.

   **Exemple de sortie console :**
   ```
   --- Statistiques Hebdomadaires ---

   Total des produits consommés : 5
   Total des produits jetés : 2

   Résumé du gaspillage :
   - Produit : Lait
     Quantité jetée : 0,5 litre
     Valeur estimée : 1,5 €

   - Produit : Pain
     Quantité jetée : 200 grammes
     Valeur estimée : 0,5 €

   Recommandations :
   - Réduisez vos achats de lait, vous jetez régulièrement ce produit.
   - Vérifiez plus souvent les dates de péremption pour éviter de jeter du pain.

   Total du gaspillage cette semaine : 2,0 €
   ```

5. **Gestion des utilisateurs :**
   - Système de profils utilisateurs pour permettre à plusieurs personnes d’utiliser l’application avec leurs propres données.

   **Exemple de sortie console :**
   ```
   --- Connexion Utilisateur ---

   Entrez votre nom d'utilisateur : alice

   Bienvenue, Alice !
   Que voulez-vous faire aujourd'hui ?
   1. Ajouter un produit
   2. Consulter l'inventaire
   3. Voir les statistiques
   4. Se déconnecter

   Choix : 
   ```

### 3. Exigences techniques

1. **Langage :** C++ (utilisation des fonctionnalités modernes du C++11 ou plus récentes).
2. **Interface :** Interface console simple.
3. **Système de fichiers :** Utilisation de fichiers pour stocker les données des utilisateurs, des produits alimentaires et des statistiques.
4. **Portabilité :** Le programme doit être compilable sous Linux et Windows.
5. **Tests :** Prévoir une série de tests pour valider le bon fonctionnement de chaque module.

### 4. Livrables

1. **Code source :** Tout le code C++ bien documenté.
2. **README.md :** Guide d'installation, d'utilisation et explication du fonctionnement de l'application.
3. **Fichiers de configuration :** Exemples de fichiers de configuration pour les utilisateurs et les produits.
4. **Rapport :** Rapport synthétique détaillant les choix techniques et les tests réalisés.
