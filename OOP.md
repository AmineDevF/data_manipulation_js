## 📋 Exercices

### 1. Héritage : Animal → Chien

Crée une classe `Animal` avec une méthode `parler()`. Ensuite, crée une classe `Chien` qui hérite de `Animal` et redéfinit la méthode `parler()` pour que le chien aboie. Exécute les deux classes et affiche leurs résultats.

*Astuce :* Vous allez utiliser l'héritage pour partager des comportements entre les classes.

### 2. Encapsulation : propriété privée

Crée une classe `Personne` avec un attribut privé `nom`. Ajoute une méthode `setNom()` pour définir le nom et une méthode `getNom()` pour le récupérer.

*Astuce :* La méthode d'accès permet de contrôler l'accès à l'attribut privé, tout en garantissant son intégrité.

### 3. Polymorphisme : parler()

Crée deux classes, `Chat` et `Oiseau`, qui ont chacune une méthode `parler()`. Écris une fonction `faireParler($animal)` qui appelle la méthode `parler()` d'un objet. Assure-toi que chaque classe a une implémentation propre.

*Astuce :* Le polymorphisme permet de traiter des objets de types différents de manière uniforme via une méthode commune.

### 4. Overriding : démarrage voiture

Crée une classe `Voiture` avec une méthode `demarrer()`. Crée une classe `VoitureDeSport` qui hérite de `Voiture` et redéfinit `demarrer()` pour afficher un message différent, comme "Vroom Vroom".

*Astuce :* L'overriding permet de redéfinir une méthode héritée pour adapter son comportement dans la classe fille.

### 5. Méthode statique : calculerArea

Crée une classe `Rectangle` avec des propriétés `largeur` et `hauteur`. Ajoute une méthode statique `calculerArea($largeur, $hauteur)` qui renvoie l'aire du rectangle.

*Astuce :* Une méthode statique appartient à la classe elle-même et non à une instance.

### 6. Constantes : définir une constante

Dans une classe `CompteBancaire`, définis une constante `TauxInteret` à 0.05. Affiche cette constante.

*Astuce :* Une constante est une valeur fixe qui ne peut pas être modifiée une fois définie.

### 7. Héritage multiple (via la composition)

Crée une classe `Employe` avec un attribut `nom`. Crée une classe `Manager` qui contient un objet `Employe` et lui affecte un nom. Affiche le nom de l'employé via le manager.

*Astuce :* Parfois, il est plus logique de composer des objets plutôt que d'hériter directement.

### 8. Encapsulation avec Getter et Setter

Crée une classe `Banque` avec un attribut `solde` privé. Utilise des méthodes `getSolde()` et `setSolde()` pour gérer l'accès à cet attribut.

*Astuce :* Utiliser des getter et setter permet de mieux contrôler l'accès aux données sensibles.

### 9. Polymorphisme avec méthode abstraite

Crée une classe `Forme` avec une méthode abstraite `calculerPerimetre()`. Crée deux classes `Cercle` et `Rectangle` qui implémentent cette méthode de manière différente.

*Astuce :* Les classes abstraites servent de modèle pour les classes dérivées.

### 10. Overloading de méthodes

Crée une classe `Calculatrice` avec une méthode `additionner()` qui accepte deux paramètres ou trois paramètres (via surcharge de méthode).

*Astuce :* PHP n'a pas de surcharge de méthode, mais vous pouvez imiter ce comportement en utilisant des arguments par défaut.

### 11. Méthodes statiques avec compteur

Crée une classe `Visiteur` avec une propriété statique `compteur` qui compte le nombre d'instances créées. Affiche le nombre d'instances après la création de chaque objet.

*Astuce :* Les variables statiques permettent de conserver des informations entre toutes les instances d'une classe.

### 12. Encapsulation et visibilité

Crée une classe `Voiture` avec une propriété `vitesse` protégée et une méthode publique `accelérer()`. Essayez de modifier directement `vitesse` depuis l'extérieur de la classe.

*Astuce :* Les propriétés protégées ne sont accessibles que dans la classe et ses enfants.

### 13. Constantes et enregistrement de type

Dans une classe `Formule1`, définis une constante `TYPE` avec la valeur "F1". Crée une méthode qui affiche ce type.

*Astuce :* Les constantes sont idéales pour les valeurs qui ne doivent pas changer durant l'exécution.

### 14. Surcharge de méthodes : vérifierSiPositif

Crée une classe `Mathematiques` avec une méthode `vérifierSiPositif()`. Surcharge cette méthode pour qu'elle accepte un nombre ou un tableau de nombres.

*Astuce :* PHP ne supporte pas nativement la surcharge de méthodes, mais vous pouvez utiliser des arguments variadiques.

### 15. Classe abstraite avec méthode concrète

Crée une classe abstraite `Ouvrage` avec une méthode concrète `decrire()`. Crée une classe `Livre` qui hérite de `Ouvrage` et redéfinit `decrire()`.

*Astuce :* Les méthodes concrètes dans une classe abstraite peuvent être partagées par les classes enfants.

### 16. Overriding avec final

Crée une classe `Animal` avec une méthode `seDeplacer()`. Dans une classe `Poisson`, redéfini `seDeplacer()`, puis utilisez `final` pour empêcher d'autres classes de redéfinir cette méthode.

*Astuce :* Le mot-clé `final` empêche la redéfinition d'une méthode dans une sous-classe.

### 17. Méthodes et arguments par défaut

Dans une classe `Calculatrice`, crée une méthode `soustraire()` qui accepte deux arguments. Si aucun argument n'est passé, la méthode doit soustraire 10 par défaut.

*Astuce :* Les arguments par défaut vous permettent de rendre vos méthodes plus flexibles.

### 18. Héritage et appels de méthodes parent

Dans une classe `Etudiant`, définis une méthode `etudier()`. Dans une classe `Doctorant`, redéfini `etudier()` et appelle la méthode `etudier()` du parent.

*Astuce :* Utilisez `parent::methode()` pour appeler une méthode définie dans la classe parente.

### 19. Méthode statique et instance

Crée une classe `Utilisateur` avec une méthode statique `creer()` qui crée une instance de `Utilisateur`. Affiche un message lorsque l'instance est créée.

*Astuce :* Les méthodes statiques sont appelées sur la classe elle-même, pas sur les objets.

### 20. Classes et constantes

Dans une classe `Banque`, définis une constante `TauxInteret` et une méthode `appliquerInteret()` qui applique ce taux au solde d'un compte. Affiche le nouveau solde après application de l'intérêt.

*Astuce :* Utiliser une constante dans un contexte d'opération financière pour assurer que les taux restent constants.
