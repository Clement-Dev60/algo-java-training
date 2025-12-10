# Ma prédiction - Exercice 19

## Partie 1 : Comprendre l'existant

### Classe `Produit`

**Attributs (noms cryptiques) :**
- `n` représente : name
- `p` représente : price
- `q` représente : quantity

**Méthode `valeur()` :**
- Que calcule-t-elle ? prix*quantité donc la valeur totale des produits

---

### Classe `Inventaire`

**Attributs :**
- `prods` représente : La liste des produits
- `nb` représente : Le nombre de produits dans l'inventaire

**Méthodes :**
- `ajouter(Produit p)` : ajoute le produit p dans le tableau si il ne dépasse pas nb (quantité max ?)
- `chercher(String nom)` : Recherche un produit grâce au nom
- `afficher()` : Affiche le nom des produits avec le prix et la quantité dispo
- `valeurTotale()` : Calcule la valeur totale de l'inventaire

---

## Partie 2 : Prédire la sortie actuelle

```
=== Inventaire ===
Pomme : 2.5 x 100
Pain : 1.2 x 50
Lait : 0.95 x 75
Beurre : 2.1 x 30

=== Recherche 'Pain' ===
Trouve : Pain a 1.2 euros

=== Valeur totale ===
Valeur : 444.25 euros
```

---

## Partie 3 : Ajouter la fonctionnalité

**Fonctionnalité demandée :** 
Ajouter une méthode `afficherCher(double seuil)` qui affiche les produits dont le prix est supérieur au seuil.

**Ma méthode :**
```java
public void afficherCher(double seuil) {
    
}
```

**Sortie attendue pour `afficherCher(2.0)` :**
```

```
