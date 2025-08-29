# Approfondissement : Topos des préfaisceaux et logique quantique (Isham–Döring)

## 1. Le topos des préfaisceaux sur les contextes

- Point de départ : une algèbre de von Neumann \(\mathcal N\) représentant les observables d’un système quantique.  
- **Contextes** : la catégorie $$\(\mathcal V(\mathcal N)\)$$ dont  
  - objets = sous-algèbres commutatives $$\(V \subset \mathcal N\)$$,  
  - morphismes = inclusions $$\(i_{V'V}: V' \hookrightarrow V\)$$.  
- **Topos associé** : $$\(\mathbf{E} := \mathbf{Set}^{\mathcal V(\mathcal N)^{op}}\)$$, la catégorie des préfaisceaux contravariants sur $$\(\mathcal V(\mathcal N)\)$$.  

Dans ce topos, les énoncés logiques ne se formulent plus dans la logique booléenne classique, mais dans la logique **intuitionniste** interne du topos.

---

## 2. Le spectral presheaf \(\Sigma\) : l’objet d’états

- À chaque contexte $$\(V\)$$, on associe son **spectre de Gelfand** $$\(\Sigma(V)\)$$, ensemble des caractères multiplicatifs $$\(V \to \mathbb{C}\)$$.  
- Pour chaque inclusion $$\(i_{V'V}\)$$, on définit la restriction  
  $$\[
  \Sigma(i_{V'V})(\lambda) = \lambda|_{V'}.
  \]$$  
- L’ensemble des $$\(\Sigma(V)\)$$, avec ces restrictions, définit le **spectral presheaf** $$\(\Sigma\)$$.  
- Fait clé : si $$\(\dim \mathcal H \geq 3\)$$, $$\(\Sigma\)$$ n’admet **aucune section globale** (aucun « point global »). C’est la traduction catégorique du **théorème de Kochen–Specker** : impossibilité d’assigner des valeurs déterminées et cohérentes à toutes les observables.

---

## 3. Propositions comme sous-objets clopens (daseinisation)

- Dans la MQ classique, une proposition « $$\(A \in \Delta\)$$ » correspond à un projecteur \(P_{A\in\Delta}\).  
- Mais $$\(P\)$$ n’appartient pas en général à un contexte abélien \(V\).  
- **Daseinisation** : on approxime $$\(P\)$$ dans chaque $$\(V\)$$ par un projecteur de $$\(V\)$$. Deux variantes :  
  - **Extérieure** :  
    $$\[
    \delta^o(P)_V = \bigwedge \{ Q \in \mathrm{Proj}(V)\ :\ P \leq Q \}.  
    \]$$  
  - **Intérieure** :  
    $$\[
    \delta^i(P)_V = \bigvee \{ Q \in \mathrm{Proj}(V)\ :\ Q \leq P \}.  
    \]$$  
- Par le théorème de Gelfand, un projecteur de \(V\) correspond à un **sous-ensemble clopen** de \(\Sigma(V)\).  
- Donc \(\delta(P)\) définit un **sous-objet clopen** de $$\(\Sigma\)$$.  
- Intuition : chaque contexte fournit une approximation cohérente de la proposition.

---

## 4. États et valeurs de vérité intuitionnistes

### États comme objets de vérité
- Un état \(\rho\) (matrice de densité) définit un **truth object** \(\mathbb T_\rho\).  
- Pour chaque contexte \(V\), \(\mathbb T_\rho(V)\) contient les propositions clopens « totalement vraies » dans \(V\) sous \(\rho\).

### Valeurs de vérité
- La valeur de vérité d’une proposition \(\delta(P)\) sous \(\rho\) est donnée par une **section globale** de l’objet classificateur \(\Omega\) :  
  $$\[
  \nu_\rho(P)\ \in\ \Gamma\Omega.
  \]$$  
- Concrètement, $$\(\nu_\rho(P)_V\)$$ est un **crible** sur $$\(V\)$$ : l’ensemble des inclusions $$\(i_{V'V}\)$$ pour lesquels la proposition est vraie dans $$\(V'\)$$.  
- Les sections globales $$\(\Gamma\Omega\)$$ forment une **algèbre de Heyting**, qui fournit la logique interne.

### Exemple (qubit)
- $$\(\mathcal H = \mathbb C^2\)$$, observable $$\(\sigma_z\)$$.  
- Proposition $$\(P_z^+\)$$ : « $$\(\sigma_z = +1\)$$ ».  
- Dans le contexte $$\(V_z = \langle \sigma_z \rangle\) : \(\delta^o(P_z^+)=P_z^+\)$$ ⇒ la proposition est **top**.  
- Dans $$\(V_x = \langle \sigma_x \rangle\) : \(P_z^+ \notin V_x\)$$, donc $$\(\delta^o(P_z^+)=\mathbb 1\), \(\delta^i(P_z^+)=0\)$$. La proposition est « toujours vraie » ou « toujours fausse » selon la variante choisie, reflétant la contextualité.

---

## 5. Mesures et règle de Born

- On définit une **mesure interne** (valuation)  
  $$\[
  \mu_\rho: \mathrm{Sub}_{cl}(\Sigma) \to [0,1]^{\leftrightarrow},
  \]$$  
  où $$\([0,1]^{\leftrightarrow}\)$$ sont des **réels généralisés** (intervalles internes).  
- Pour un projecteur $$\(P_{A\in\Delta}\)$$ associé à une observable $$\(A\)$$,  
  $$\[
  \mu_\rho(\delta(P_{A\in\Delta})) = \mathrm{tr}(\rho P_{A\in\Delta}),
  \]$$  
  ce qui récupère la **règle de Born**.

---

## 6. Logique de Heyting

- L’ensemble des sous-objets clopens de \(\Sigma\) forme une **algèbre de Heyting** interne.  
- Les connecteurs (et, ou, implication) y sont **distributifs**, contrairement à la logique orthomodulaire usuelle des projecteurs.  
- Ainsi, l’« étrange logique quantique » devient une **logique intuitionniste distributive** parfaitement intégrée au cadre topos.

---

## 7. Intérêt pour les CFS

- Les **Causal Fermion Systems (CFS)** nécessitent une structure d’espace d’états et une notion de mesure universelle.  
- Le **spectral presheaf** et les valuations internes offrent un cadre naturel pour reformuler ces notions.  
- Les relations causales et l’action peuvent alors être définies **en interne**, en cohérence avec la logique intuitionniste.  
- On obtient une alternative au multivers : un **univers unique**, mais dont la logique est contextuelle et distributive.

---
