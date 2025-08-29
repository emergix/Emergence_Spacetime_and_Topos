# Visualisation d’algèbres de Heyting simples

## 1) Exemple booléen : sous-ensembles de {1,2}

Considérons l’ensemble $$\(\{1,2\}\)$$.  
L’algèbre des parties $$\(\mathcal{P}(\{1,2\})\)$$ est une **algèbre de Boole**, donc aussi une **algèbre de Heyting**.

Ordre = inclusion.  
$$\(\bot = \varnothing\), \(\top = \{1,2\}\)$$.

```
        {1,2}  =  ⊤
        /   \
     {1}    {2}
        \   /
         ∅      =  ⊥
```

- **Meet** (∧) = intersection  
- **Join** (∨) = union  
- **Implication** : $$\(A ⇒ B\) = \(\neg A \cup B\)$$ (comme dans la logique classique).  

Exemples :  
- $$\(\{1\} ⇒ \{1,2\} = \top\)$$  
- $$\(\{1\} ⇒ \{2\} = \{2\}\)$$  
- $$\(\{1\} ⇒ \varnothing = \{2\}\)$$  

Ici, la structure ressemble à un **petit arbre**, mais c’est en fait un **treillis** : les branches se rejoignent.

---

## 2) Exemple non booléen : ouverts de l’espace de Sierpiński

Espace $$\(X = \{0,1\}\)$$ avec topologie $$\( \{\varnothing, \{1\}, \{0,1\}\}\)$$.  
C’est l’exemple canonique d’un espace topologique non trivial dont les ouverts forment une algèbre de Heyting **non booléenne**.

```
      {0,1}  =  ⊤
        |
       {1}
        |
        ∅     =  ⊥
```

Opérations :  
- $$\(U ∧ V = U \cap V\)$$  
- $$\(U ∨ V = U \cup V\)$$  
- **Implication intuitionniste** : $$\(U ⇒ V\)$$ = le plus grand ouvert $$\(W\)$$ tel que $$\(U∧W \subseteq V\)$$.  

Exemples :  
- $$\(\{1\} ⇒ \varnothing = \varnothing\)$$  
- $$\(\{1\} ⇒ \{1\} = \top\)$$  
- $$\(\top ⇒ \{1\} = \{1\}\)$$  
- $$\(\top ⇒ \varnothing = \varnothing\)$$  

Ici, il n’y a pas de complément classique : $$\(\{1\}\)$$ n’a pas de complément ouvert.  
C’est une véritable **Heyting-algèbre intuitionniste**.

---

## Conclusion

- Une **algèbre de Heyting** est toujours un **treillis distributif** avec $$\(\bot\)$$, $$\(\top\)$$ et implication interne.  
- Certaines (comme les algèbres de parties finies) sont aussi booléennes : elles ressemblent à des arbres.  
- Mais en général (comme les ouverts d’un espace topologique), la structure **n’est pas un arbre**, mais un **treillis** : plusieurs chemins logiques peuvent se rejoindre.

