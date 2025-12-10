# Ma prédiction - Exercice 15

## Fonction `trouverMax`

```java
int max = ???;      // Trou 1 : t[0]
for (int i = ???;   // Trou 2 : 1
    if (t[i] ??? max)  // Trou 3 : >
        max = ???;     // Trou 4 : t[i]
```

**Raisonnement :**
- Trou 1 : On prend la première valeur du tableau pour commencer
- Trou 2 : On part de i = 1 car on a déjà la première valeur du tableau donc inutile de la comparer à elle même
- Trou 3 : Si t[i] est supérieur au maximum actuel c'est ce qu'on cherche
- Trou 4 : On remplace max par t[i] s'il est plus grand

---

## Fonction `contient`

```java
if (??? == ???)     // Trou 1 et 2 : t[i] == val
    return ???;     // Trou 3 : true
return ???;         // Trou 4 : false
```

**Raisonnement :**
- Trous 1-2 : On cherche à savoir si la valeur est dans le tableau donc on compare chaque valeur du tableau avec val
- Trou 3 : Si c'est le cas on renvoie Vrai
- Trou 4 : Sinon c'est faux

---

## Fonction `sommePairs`

```java
if (t[i] ??? 2 == ???)  // Trou 1 et 2 : % et 0
    somme = somme + ???; // Trou 3 : t[i]
```

**Raisonnement :**
- Trou 1 : On utilise le modulo de deux pour savoir si c'est pair ou non grâce au reste
- Trou 2 : Si c'est égal à 0 alors c'est pair
- Trou 3 : On ajoute à la somme la valeur de t[i] s'il est pair

---

## Fonction `dupliquer`

```java
int[] res = new int[t.length ??? 2];  // Trou 1 : *
res[i ??? 2] = t[i];                   // Trou 2 : *
res[i ??? 2 ??? 1] = t[i];              // Trou 3 et 4 : * et +
```

**Raisonnement :**
- Trou 1 : On double la taille de la liste pour pouvoir la dupliquer
- Trou 2 : On multiplie l'indice de res par 2 car tout est décalé comme on duplique (t[1] sera égal à res[2])
- Trous 3-4 : On multiplie l'indice de res par 2 toujours pour décaler et on ajoute un pour prendre celui d'après afin de le dupliquer
