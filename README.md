⚡ Fun fact: **Zygohistomorphic prepromorphisms** - Zygo implements semi-mutual recursion like a zygomorphism. Para gives you access to your result à la paramorphism.
```haskell
zygoHistoPrepro 
  :: (Unfoldable t, Foldable t) 
  => (Base t b -> b) 
  -> (forall c. Base t c -> Base t c) 
  -> (Base t (EnvT b (Stream (Base t)) a) -> a) 
  -> t
  -> a
```
