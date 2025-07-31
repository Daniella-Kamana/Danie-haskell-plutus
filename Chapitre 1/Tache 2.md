HC1T2 - Tâche 2 : Exemple de fonction pure

```haskell
-- Fonction pure : calcul de l'aire d'un cercle
aireCercle :: Floating a => a -> a
aireCercle rayon = pi * rayon * rayon

-- Fonction principale
main :: IO ()
main = do
    let rayon = 5.0
    let aire = aireCercle rayon
    putStrLn ("L'aire d'un cercle de rayon " ++ show rayon ++ " est " ++ show aire)

```

### Explication :

* `aireCercle` est l’équivalent de `circleArea`.
* Les messages sont en français.
* Le programme calcule l’aire d’un cercle de rayon 5.0 et affiche le résultat.

