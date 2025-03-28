# MyGest IOn'R


**MyGest IOn'R** est un programme en **Bash** permettant de gérer un parc informatique en utilisant une base de données MariaDB. Il offre une série d'outils permettant d'ajouter, supprimer, afficher et modifier des équipements informatiques et leurs types. Ce projet est destiné à faciliter la gestion des équipements réseau pour les administrateurs système et réseau.

## Fonctionnalités

1. **Gestion des équipements** :
    - Ajouter un type de matériel (Table TypeE).
    - Ajouter une machine à l'inventaire (Table Equipement).
    - Afficher les équipements et les types de matériels.
    - Modifier les informations des équipements et des types de matériels.
    - Supprimer des équipements et des types de matériels.

2. **Base de données** :
    - La base de données utilisée est **MariaDB**.
    - Elle contient deux tables :
      - `TypeE` : pour les types de matériel.
      - `Equipement` : pour les équipements informatiques.

3. **Interface Menu** :
    - Un menu interactif permet à l'utilisateur de choisir parmi plusieurs options : afficher, ajouter, supprimer ou modifier des données.


## Installation

1. **Cloner le repository** :
   Clonez ce repository sur votre machine locale :

   ```bash
   git clone https://github.com/Oursin2Mer/MyGestion-R.git
   cd MyGestion-R
   ```

2. **Exécution du script principal** :
   - Le script principal, `script.sh`, est un fichier Bash qui gère toutes les opérations.
   - Il installe également la base de données et configure les tables nécessaires la première fois qu'il est exécuté.

   Pour démarrer le programme, exécutez le script :

   ```bash
   ./script.sh
   ```

3. **Configurer la base de données** :
   Le script crée automatiquement une base de données MariaDB appelée **MyGest** et y ajoute les tables nécessaires.

## Utilisation

Le programme propose un menu interactif avec les options suivantes :

1. **Afficher la base de données** :
   Vous pouvez afficher les équipements et les types de matériels dans la base de données.

2. **Ajouter des données** :
   - Ajouter un type de matériel.
   - Ajouter une machine à l'équipement actif.

3. **Supprimer des données** :
   - Supprimer un type de matériel de l'inventaire.
   - Supprimer une machine de l'équipement actif.

4. **Modifier des données** :
   - Modifier les informations d'un équipement (nom, MAC, IP, etc.).
   - Modifier les informations d'un type de matériel.

5. **Quitter** :
   Quittez le programme.

Le menu s'affiche en boucle jusqu'à ce que l'utilisateur choisisse de quitter le programme.
