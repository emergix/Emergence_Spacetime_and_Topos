# Topos et Physique Quantique

## 1. Motivation : le problème de la mesure

En mécanique quantique standard :  
- L’évolution est unitaire (équation de Schrödinger).  
- La mesure nécessite un **postulat du collapse**, extérieur à la dynamique.  
- Alternatives :  
  - **Multivers (Everett)** : tous les résultats coexistent dans des branches parallèles.  
  - **Topos** : reformuler la logique et l’ontologie, sans multiplier les mondes.

## 2. Idée de base de l’approche topos

- Utiliser la **théorie des topos** pour reformuler la logique quantique.  
- Principe : remplacer l’espace d’états classique par un **objet d’états interne** à un topos.  
- Les valeurs de vérité ne sont plus booléennes \(\{0,1\}\), mais appartiennent à une **algèbre de Heyting** (logique intuitionniste).  

**Conséquence :**  
- Pas besoin de collapse.  
- Les propositions sont évaluées dans une logique distributive mais non-classique.  
- La « multiplicité » des mondes devient une **contextualité logique**, non une ontologie parallèle.

## 3. Construction (Isham–Döring, Heunen–Landsman–Spitters)

1. **Système quantique** : algèbre de von Neumann \(\mathcal N\) des observables.  
2. **Contextes** : catégorie \(\mathcal V(\mathcal N)\) des sous-algèbres **abéliennes** de \(\mathcal N\).  
3. **Topos** : catégorie des préfaisceaux \(\mathbf{Set}^{\mathcal V(\mathcal N)^{op}}\).  
4. **Objet d’états** : le **spectral presheaf** \(\Sigma\).  
   - Pas de sections globales (↔ théorème de Kochen–Specker).  
5. **Propositions** : les projecteurs \(P\) sont envoyés vers des sous-objets de \(\Sigma\) (via la **daseinisation**).  
6. **États et vérités** : un état \(\rho\) définit un **truth object** qui assigne des valeurs de vérité intuitionnistes (cribles sur les contextes).  

## 4. Exemple : le qubit

- Observables : \(\sigma_x, \sigma_y, \sigma_z\).  
- Contextes : algèbres engendrées par chacun.  
- Proposition « \(\sigma_z = +1\) » : projecteur \(P_z^+\).  
- Sa daseinisation est vraie (top) dans les contextes contenant \(\sigma_z\), et « partiellement vraie » ailleurs (valeur Heyting).  
- La mesure est alors une **mise à jour interne** du truth object, non un collapse externe.

## 5. Comparaison avec le multivers

| Aspect | Multivers (Everett) | Topos quantique |
|--------|---------------------|-----------------|
| Ontologie | Tous les mondes existent réellement | Un seul monde, mais logique interne non booléenne |
| Logique | Classique globale | Intuitionniste (Heyting), contextuelle |
| Mesure | Décohérence + branchement | Conditionnement interne (truth object) |
| Testabilité | Peut-être via gravité quantique | Expériences de contextualité, logique interne |

## 6. Avantages de l’approche topos

- Évite le postulat du collapse.  
- Évite la prolifération ontologique des multivers.  
- Donne une logique distributive, adaptée aux propositions quantiques.  
- Fournit un cadre catégorique riche, unifiant logique et géométrie.

## 7. Limites et perspectives

- Traitement des probabilités (règle de Born) encore en discussion.  
- Dynamique et mesures séquentielles : sujets de recherche active.  
- Lien avec la gravité quantique et la cosmologie : pistes ouvertes.

---

## Bibliographie sélective

- J. Butterfield & C.J. Isham, *A topos perspective on the Kochen–Specker theorem: I–VI*, International Journal of Theoretical Physics, 2000–2002.  
- C.J. Isham & A. Döring, *A topos foundation for theories of physics: I–IV*, Journal of Mathematical Physics, 2007.  
- A. Döring & C.J. Isham, *What is a Thing? Topos Theory in the Foundations of Physics*, arXiv:0803.0417 (2008).  
- C. Heunen, N.P. Landsman, B. Spitters, *A topos for algebraic quantum theory*, Communications in Mathematical Physics 291 (2009).  
- A. Döring, *Topos theory and ‘neo-realist’ quantum theory*, in *New Structures for Physics*, Lecture Notes in Physics 813 (2011).  
- S. Abramsky & A. Brandenburger, *The sheaf-theoretic structure of non-locality and contextuality*, New Journal of Physics 13 (2011).  

---

**Résumé final :**  
Les **topos quantiques** offrent une alternative élégante au multivers pour le problème de la mesure.  
Ils reformulent la mécanique quantique dans une logique intuitionniste interne, où la contextualité et l’absence de valeurs globales remplacent la prolifération de mondes parallèles.
