HC1T1 - Tâche 1 : Composition de fonctions

---

### ✅ Code Haskell fonctionnel

```haskell
-- Définition des fonctions

-- Multiplie un nombre par 2
double :: Int -> Int
double x = x * 2

-- Augmente un nombre de 1
increment :: Int -> Int
increment x = x + 1

-- Applique double puis increment, en utilisant la composition
doubleThenIncrement :: Int -> Int
doubleThenIncrement = increment . double

-- Fonction principale pour tester
main :: IO ()
main = do
    print (double 4)              -- Affiche 8
    print (increment 8)           -- Affiche 9
    print (doubleThenIncrement 4) -- Affiche 9

```

---

### 📘 Explications

#### 1. `double`

```haskell
double x = x * 2
```

* Cette fonction prend un entier `x` et retourne `x` multiplié par 2.
* Exemple : `double 3` donne `6`.

#### 2. `increment`

```haskell
increment x = x + 1
```

* Elle prend un entier `x` et retourne `x + 1`.
* Exemple : `increment 6` donne `7`.

#### 3. `doubleThenIncrement`

```haskell
doubleThenIncrement = increment . double
```

* Cette ligne signifie **"compose les fonctions"**.
* `(f . g)` signifie appliquer d’abord `g`, ensuite `f`.
* Donc ici, `doubleThenIncrement x = increment (double x)`.

---

### ✅ Exemple d'utilisation dans GHCi

```haskell
ghci> double 4
8

ghci> increment 8
9

ghci> doubleThenIncrement 4
9
```

---


Si tu veux, je peux t’aider à faire un petit programme complet avec `main` pour tester cela. Souhaites-tu cela ?
