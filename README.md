# Éditeur de Compte Bancaire

L'Éditeur de Compte Bancaire est une application Java conçue pour gérer facilement vos comptes bancaires. Elle permet d'ajouter, modifier et supprimer des opérations tout en calculant automatiquement les soldes.

## Prérequis

- **Java Development Kit (JDK)** : Installez la version 16 ou supérieure.

## Installation et Lancement

1. **Téléchargez et extrayez l'archive** : `Editeur_Compte_Bancaire.zip` où vous le souhaitez.
2. Une fois extrait, accédez au dossier `Editeur de compte bancaire`. Ce dernier contient :
   - `Lancer_Editeur_de_compte_bancaire.bat`
   - `EditeurCompteBancaire.jar`
3. **Pour lancer l'application**, exécutez le fichier EditeurCompteBancaire.jar à l’aide de Java. Veillez à ce que le fichier soit bien ouvert avec Java et non avec un gestionnaire d’archives tel que WinRAR, qui est parfois sélectionné par défaut.

## Fonctionnement de l'application

### Interface Principale
- **Boutons principaux** :
  - **Ajouter** : Ouvre une fenêtre pour ajouter une opération.
  - **Modifier** : Permet de modifier une opération sélectionnée.
  - **Supprimer** : Supprime une opération sélectionnée.

- **Menu « Fichier »** :
  - **Nouveau** : Démarrer un nouveau compte.
  - **Ouvrir** : Ouvrir un fichier existant.
  - **Enregistrer** : Enregistrer les modifications (ou enregistrer sous si aucun fichier n'a été ouvert).
  - **Enregistrer Sous** : Enregistrer les données dans un nouveau fichier.
  - **Quitter** : Fermer l'application.

### Ajout d'une opération
1. **Choisir** : Débit ou Crédit.
2. **Sélectionner** : La date, le type de paiement, et la catégorie.
3. **Saisir** : Libellé et montant (le format décimal avec point `.` est requis).
4. **Cocher** : Si l’opération est pointée.

Boutons :
- **Réinitialiser** : Remet le formulaire à zéro.
- **Valider** : Ajoute l'opération. Si des informations sont manquantes ou invalides, un message d'erreur sera affiché.

### Modification d'une opération
Fonctionne comme l'ajout avec les différences suivantes :
- **Réinitialiser** : Recharge les données initiales de l'opération.
- **Valider** : Modifie l'opération existante avec les nouvelles informations.

### Informations supplémentaires
- Le solde est **calculé automatiquement**.
- Les débits sont affichés en **rouge** et les crédits en **vert**.
- Les opérations peuvent être modifiées directement dans le tableau.

## Format des fichiers pris en charge

L'application accepte des fichiers texte, mais le format recommandé est **CSV** avec les colonnes suivantes :
1. Date (format `JJ/MM/AAAA`).
2. Type de paiement (ex. CB, Espèces, Chèque, etc.).
3. Libellé.
4. Catégorie (correspondant à la liste prédéfinie).
5. Montant (avec un point `.` comme séparateur décimal).
6. Pointage (`oui` ou `non`).

### Catégories disponibles
#### Débits :
- Achats & Shopping, Alimentation & Restaurants, Logement & Charges, etc.
#### Crédits :
- Salaires, Revenus complémentaires, Économies, etc.
#### Autres :
- Non catégorisé, Autre.

## Notes
- Attention aux apostrophes spécifiques et espaces invisibles pouvant provoquer des erreurs.
- Évitez de modifier le format du fichier en dehors de l'application.

---

**Besoin d'aide ?** Consultez la documentation incluse dans l'archive.
