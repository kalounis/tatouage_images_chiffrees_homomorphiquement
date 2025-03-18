# Projet: Tatouage d’images chiffrées homomorphiquement

Ce projet s'inscrit dans le cadre de l'UE Cryptologie avancée et protection des données de la TAF CYBER à IMT Atlantique.

L'objectif est de tatouer des messages dans le domaine clair et dans le domaine chiffré d'une image chiffrée homomorphiquement avec le cryptosystème de Paillier.

Le projet consiste en un notebook python .ipynb séparé en différentes parties :
- I. Préparation : Import des modules python nécessaires
- II. Fonction cryptographiques (Paillier) : Définition des fonctions de chiffrement et déchiffrement de Paillier
- III. Fonctions de transformation (image / liste 2D / vecteur 1D) : Définition des fonctions qui transforment l'image en vecteur unidimentionnel et inversement
- IV. Pre-marque : Insertion d'une pré-marque dans l'image, afin de permettre l'extraction du message tatoué dans le domaine clair de l'image
- V. Chiffrement de l'image : Chiffrement homomorphique de l'image avec la méthode de Paillier
- VI. Transformation (message en texte / message en bits) : Définition des fonctions qui traduissent un message textuel en liste de bits et inversement
- VII. Insertion d'un message dans le domaine clair de l'image : Insertion d'un premier message ("James Bond est un agent secret") dans le domaine clair de l'image. Test d'extraction du message à partir de l'image.
- VIII. Insertion d'un message dans le domaine chiffré de l'image : Insertion d'un deuxième message ("Astron Martin") dans le domaine chiffré de l'image. Test d'extraction du message à partir de l'image.
- IX. Exctraction du message en clair, après avoir ajouté le tatouage dans le domaine chiffré : Test d'extraction du premier message (dans le domaine clair de l'image), maintenant que le deuxième message a été tatoué dans le domaine chiffré de l'image, pour vérifier qu'il est toujours possible de l'extraire.
- X. Bonus : Reconstruction de l'image, à partir du vecteur tatoué