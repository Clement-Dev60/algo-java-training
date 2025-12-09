# Ma prédiction - Exercice 14

## BUG 1 : fonction `moyenne`

**Ligne suspecte :** 28, for (int i = 0; i <= t.length; i++)

**Description du bug :** Dans un tableau de longueur t.length, les indices valides vont de 0 à t.length -1

**Ce qui va se passer :** On va recevoir un erreur d'indexoutofbounds

**Correction proposée :** for (int i = 0; i <= t.length-1; i++)

---

## BUG 2 : fonction `estTrie`

**Ligne suspecte :** 37 t[i + 1]

**Description du bug :** À la fin de la boucle, on accède à un indice qui n’existe pas

**Ce qui va se passer :** On va recevoir un erreur d'indexoutofbounds

**Correction proposée :** for (int i = 0; i < t.length - 1; i++) {
if (t[i] > t[i+1]) {return false;};
}

---

## BUG 3 : fonction `inverse`

**Ligne suspecte :** 46 for (int i = 0; i < t.length; i++)

**Description du bug :** La boucle fait sur toute la longueur de la liste

**Ce qui va se passer :** Elle va inverser une fois ok mais elle va tout remettre comme au début après

**Correction proposée :** for (int i = 0; i < t.length / 2; i++)

---

## BUG 4 : fonction `compter`

**Ligne suspecte :** 59 if (t[i] == val) {
count++;
return count;
}

**Description du bug :** Le return count est dans la boucle

**Ce qui va se passer :** Il va mettre fin à l'exécution à la première occurrence

**Correction proposée :** if (t[i] == val) {
count++;
}
