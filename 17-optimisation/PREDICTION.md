# Ma prédiction - Exercice 17

## Fonction `moyenneInef`

**Problème identifié :** Faire une double boucle for est inutile + remettre la somme à 0 à chaque

**Nombre d'opérations actuelles (pour n éléments) :** (n\*(n+1))/2

**Version optimisée :**

```java
public static double moyenneEff(int[] t) {
    if (t == null || t.length == 0) return 0;

    double somme = 0;
    for (int i = 0; i < t.length; i++) {
        somme += t[i];
    }
    return somme / t.length;
}
```

---

## Fonction `contientDoublonInef`

**Problème identifié :** Initalisation de j à 0 et vérification si i != j

**Version optimisée :**

```java
 public static boolean contientDoublon(int[] t) {
    for (int i = 0; i < t.length; i++) {
        for (int j = i + 1; j < t.length; j++) {
            if (t[i] == t[j]) {
                return true;
            }
        }
    }
    return false;
}
```

---

## Fonction `premierEtDernierInef`

**Problème identifié :** boucles for inutiles

**Version optimisée :**

```java
public static String premierEtDernier(int[] t) {
    int premier = t[0];
    int dernier = t[t.length - 1];
    return premier + " et " + dernier;
}
```

---

## Fonction `rechercheInef`

**Problème identifié :** Ne s'arrête pas même s'il l'a trouvé

**Version optimisée :**

```java
public static int rechercheInef(int[] t, int val) {
        for (int i = 0; i < t.length; i++) {
            if (t[i] == val) {
                return i
            }
        }
        return -1;
    }
```
