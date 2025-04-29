

# 🧠 10 Exercices PHP Orienté Objet — *Pratiques de 5 minutes*



## ✅ 1. Héritage → `Dog` hérite de `Animal`

> **Contexte** : Dans un zoo, chaque animal produit un son spécifique.  
> **Consigne** : Créer une classe `Dog` qui hérite de `Animal` et redéfinit `sound()`.

```php
$dog = new Dog();
echo $dog->sound(); // Woof!
```

---

## ✅ 2. Polymorphisme → `Shape` → `Circle`, `Square`

> **Contexte** : Calcul d’aires de formes.  
> **Consigne** : Implémentez `Shape` avec les classes `Circle` et `Square`.

```php
$circle = new Circle(3);
$square = new Square(4);
echo $circle->area(); // ~28.27
echo $square->area(); // 16
```

---

## ✅ 3. Encapsulation → `BankAccount`

> **Contexte** : Éviter les soldes négatifs.  
> **Consigne** : Empêcher l’attribution d’un solde négatif via un setter.

```php
$account = new BankAccount();
$account->setBalance(100); // OK
$account->setBalance(-50); // Exception: "Solde invalide!"
```

---

## ✅ 4. Override → `ElectricCar` hérite de `Vehicle`

> **Contexte** : Les voitures électriques n’utilisent pas de moteur thermique.  
> **Consigne** : Redéfinir la méthode `start()`.

```php
$car = new ElectricCar();
echo $car->start(); // "Battery activated"
```

---

## ✅ 5. Méthode statique → `MathUtils::sum`

> **Contexte** : Outils de calculs mathématiques.  
> **Consigne** : Créer une méthode statique `sum($a, $b)`.

```php
echo MathUtils::sum(3, 5); // 8
```

---

## ✅ 6. Constante → `Config::APP_VERSION`

> **Contexte** : Centraliser la version de l'application.  
> **Consigne** : Déclarer une constante `APP_VERSION`.

```php
echo Config::APP_VERSION; // "1.0"
```

---

## ✅ 7. Héritage + logique → `DoubleCounter`

> **Contexte** : Incrémenter de 2 au lieu de 1.  
> **Consigne** : Surcharger `increment()` pour doubler l’incrément.

```php
$counter = new DoubleCounter();
$counter->increment();
echo $counter->getCount(); // 2
```

---

## ✅ 8. Polymorphisme + logique → `Sorter`

> **Contexte** : Tri de données en deux ordres possibles.  
> **Consigne** : Créer `AscSorter` et `DescSorter` avec `sort()`.

```php
$data = [3, 1, 4];
print_r((new AscSorter())->sort($data));  // [1, 3, 4]
print_r((new DescSorter())->sort($data)); // [4, 3, 1]
```

---

## ✅ 9. Statique + logique → `IDGenerator::generate`

> **Contexte** : Génération d’identifiants uniques.  
> **Consigne** : Implémenter une méthode statique qui s’auto-incrémente.

```php
echo IDGenerator::generate(); // 1
echo IDGenerator::generate(); // 2
```

---

## ✅ 10. Encapsulation + validation → `User::setEmail`

> **Contexte** : Valider les emails.  
> **Consigne** : Utiliser `filter_var` dans le setter `setEmail()`.

```php
$user = new User();
$user->setEmail("test@example.com"); // OK
$user->setEmail("invalid"); // Exception: "Email invalide!"
```

---

## 🛠️ Bonus : Exemple de solution pour l’exercice 1

```php
class Animal {
    public function sound() {
        return "Some sound";
    }
}
class Dog extends Animal {
    public function sound() {
        return "Woof!";
    }
}
```

