# Comment les principes de la mécanique quantique subsistent dans un **topos intuitionniste**

Ce document montre comment reformuler les **principes de la mécanique quantique (MQ)** dans la **logique intuitionniste** interne d’un topos, sans recourir au multivers ni au postulat de collapse. L’idée centrale est de remplacer l’espace d’états « global » par un **objet d’états interne** et les valeurs de vérité booléennes par des **valeurs de vérité Heyting** (cribles).

---

## 1) Dictionnaire de traduction (classique → topos)

| MQ standard (Hilbert) | Reformulation interne au topos (contravariante/presheaves) |
|---|---|
| Espace d’états (rayons de Hilbert) | **Spectral presheaf** \(\Sigma\) (associe à chaque contexte abélien son spectre de Gelfand) |
| Propositions \(P\) (projecteurs) | Sous-objets **clopens** de \(\Sigma\) via **daseinisation** \(\delta(P)\) |
| Observables auto-adjointes \(\hat A\) | Flèches internes \(\breve A:\Sigma \to \mathbb{R}^{\leftrightarrow}\) (objet « réels » d’intervalles) |
| États \(\rho\) | **Truth object** \(\mathbb T_\rho\) / pseudo-état (sélectionne les sous-objets vrais) |
| Valeurs de vérité | Sections globales de \(\Omega\) (algèbre de **Heyting**) : cribles sur les contextes |
| Logique des propositions | **Intuitionniste distributive** (Heyting), pas booléenne |
| Mesure/collapse | **Mise à jour interne** (conditionnement du truth object), pas de postulat externe |
| Dynamique unitaire | Action naturelle de *-automorphismes sur \(\Sigma\) et sur \(\breve A\) (Heisenberg/Schrödinger internes) |

**Remarque clef :** \(\Sigma\) n’a **pas** de section globale (↔ Kochen–Specker). La « non-valeur » globale devient **contextualité** plutôt que multivers.

---

## 2) Principes quantiques et leur persistance dans le topos

### (A) Superposition & interférences
- **Standard :** linéarité de l’espace de Hilbert, superpositions \(\alpha\lvert\psi\rangle+\beta\lvert\phi\rangle\).
- **Topos :** la structure linéaire est **locale** à chaque contexte (où tout est commutatif). L’« état » global étant remplacé par \(\Sigma\), les effets de superposition se lisent via la **daseinisation** des projecteurs et les **valeurs Heyting** non triviales (qui codent le degré/contextualité de vérité). Les **interférences** apparaissent par le **raffinement de contextes** et la variation des valeurs de vérité à travers eux.

### (B) Observables & spectre
- **Standard :** observable \(\hat A\) ↔ spectre \(\mathrm{sp}(\hat A)\), projecteurs spectraux.
- **Topos :** \(\breve A:\Sigma \to \mathbb{R}^{\leftrightarrow}\) associe à chaque état contextuel un **intervalle** de valeurs (approximations intérieure/extérieure). Les projecteurs spectraux \(P_{A\in\Delta}\) deviennent \(\delta(P_{A\in\Delta})\subseteq\Sigma\).

### (C) Propositions logiques
- **Standard :** propositions \((A\in\Delta)\) évaluées en \(\{0,1\}\).
- **Topos :** \(\llbracket A\in\Delta\rrbracket_\rho \in \Gamma\Omega\) est un **crible** (valeur Heyting) : l’ensemble des contextes au-dessus desquels la proposition devient vraie. La logique est **distributive** (avantage par rapport à l’orthomodularité).

### (D) Probabilités & règle de Born
- **Standard :** \( \Pr_\rho(A\in\Delta)=\mathrm{tr}(\rho\,P_{A\in\Delta}) \).
- **Topos :** on définit une **mesure interne** \(\mu_\rho:\mathrm{Sub}_{cl}(\Sigma)\to[0,1]^{\leftrightarrow}\) sur les sous-objets clopens (monotone, \(\sigma\)-additive au sens interne). La valeur \(\mu_\rho(\delta(P_{A\in\Delta}))\) **reconstruit Born** (dans les présentations standard de l’approche contravariante).

### (E) Mesure & mise à jour (sans collapse)
- **Standard :** projection post-mesure (Lüders), non unitaire.
- **Topos :** la mesure est une **révision conditionnelle interne** : l’issue « oui » pour \(P\) raffine \(\mathbb T_\rho\) en \(\mathbb T_{\rho|P}\), ce qui rend \(\delta(P)\) **vraie** (top) dans les contextes pertinents, sans postuler une discontinuité ontologique.

### (F) Incertitude & non-commutation
- **Standard :** \(\Delta A\,\Delta B \ge \frac12|\langle[\hat A,\hat B]\rangle|\).
- **Topos :** l’incompatibilité se voit par l’**absence de contexte commun** rendant simultanément \(\delta(P_{A\in\Delta_A})\) et \(\delta(P_{B\in\Delta_B})\) globalement vraies. Les **intervalles** \(\mathbb{R}^{\leftrightarrow}\) encodent une **précision finie** interne qui reflète les bornes d’incertitude.

### (G) Non-localité & contextualité
- **Standard :** violations de Bell, non-localité.
- **Topos :** recadrées comme **contextualité** (pas de global section). Les valeurs de vérité Heyting et la cohomologie de préfaisceaux (dans des cadres voisins) rendent compte des obstructions (ex. scénarios CHSH comme **obstructions de recollement**).

### (H) Dynamique unitaire
- **Standard :** \(U_t=e^{-iHt}\) agit par conjugaison sur observables ou sur états.
- **Topos :** les *-automorphismes de \(\mathcal N\) induisent des **transformations naturelles** de \(\Sigma\) et des flèches \(\breve A\). On obtient des versions internes des images de Heisenberg/Schrödinger. La **réversibilité** est donc préservée **avant** conditionnement.

### (I) Systèmes composés & intrication (⚠️ subtil)
- **Standard :** produit tensoriel \( \mathcal H_{AB}=\mathcal H_A\otimes\mathcal H_B \).
- **Topos :** la composition n’est **pas triviale** (le topos des contextes de \(AB\) n’est pas simplement le produit de ceux de \(A\) et \(B\)). L’**intrication** persiste mais se manifeste comme **obstruction de sections globales** sur le système composite. Divers schémas existent (bohrification, produits de Foulis–Randall, cadres faisceautiques) — domaine encore actif de recherche.

---

## 3) Formules-types (internes)

- **Valeur de vérité** d’une proposition sous \(\rho\) :  
  \[
  \nu_\rho(A\in\Delta)\;=\;\llbracket\,\delta(P_{A\in\Delta})\in \mathbb T_\rho\,\rrbracket \;\in\; \Gamma\Omega.
  \]
- **Mesure interne (Born)** :  
  \[
  \mu_\rho:\mathrm{Sub}_{cl}(\Sigma)\to[0,1]^{\leftrightarrow},\qquad
  \mu_\rho\big(\delta(P_{A\in\Delta})\big)\;\simeq\;\mathrm{tr}(\rho\,P_{A\in\Delta}).
  \]
- **Observable interne** :  
  \[
  \breve A:\Sigma\longrightarrow \mathbb{R}^{\leftrightarrow},\quad
  \text{valeur contextuelle = intervalle d’approximation (inner/outer)}.
  \]

---

## 4) Mini-cas d’école : qubit

1. \(\mathcal N=\mathcal B(\mathbb C^2)\). Contextes : \(\langle\sigma_x\rangle,\langle\sigma_y\rangle,\langle\sigma_z\rangle,\dots\)  
2. Proposition \(P_z^+\) (« \(\sigma_z=+1\) ») → \(\delta(P_z^+)\subseteq\Sigma\).  
3. État \(\rho=\lvert 0\rangle\langle 0\rvert\) rend \(\nu_\rho(\sigma_z{=}+1)\) **top** dans \(\langle\sigma_z\rangle\) et **partiellement vrai** ailleurs.  
4. Après issue \(+1\), mise à jour \(\mathbb T_\rho\rightsquigarrow \mathbb T_{\rho|P_z^+}\) : pas de collapse postulé, mais **vérité contextualisée** devenue top dans les contextes adéquats.

---

## 5) Ce qui est **préservé**, ce qui **change**

- **Préservé :** unitarité avant mesure, spectres et relations fonctionnelles, principe de superposition (local/contextuel), règle de Born (comme mesure interne), incompatibilité/inégalités d’incertitude, phénomènes de contextualité/intrication (reformulés en obstructions).  
- **Change :** logique **non booléenne** (Heyting), vérité **contextuelle graduée** (cribles), absence de valeurs simultanées globales, **mesure = conditionnement interne** plutôt que collapse externe.  
- **Statut ontologique :** pas de multiplication des mondes ; une seule structure interne avec logique appropriée.

---

## 6) Points ouverts (pour aller plus loin)
- Composition générale des systèmes et produits tensoriels internes.  
- Traitement uniforme des mesures séquentielles et canaux quantiques (CPTP) dans le topos.  
- Ponts avec information quantique (protocoles) et gravité quantique (localité/covariance internes).

---

### TL;DR
Les **principes quantiques** survivent au passage au topos : on garde l’unitarité, Born, incompatibilités, intrication — mais **reframed** dans une **logique intuitionniste contextuelle**. La « réduction » devient une **mise à jour interne** des vérités, sans multivers ni collapse postulé.

---

## Schéma du flux logique (Mermaid)

```mermaid
flowchart LR
  A[Etat rho (truth object)] --> B[Proposition<br/>daseinisation: delta(P_{A in Delta})]
  B --> C[Evaluation<br/>valeur de verite<br/>nu_rho(A in Delta) in Gamma(Omega)]
  C --> D{Mesure / issue ?}
  D -- oui --> E[Mise a jour interne<br/>T_rho => T_{rho|P}]
  D -- non --> F[Evolution unitaire interne<br/>(automorphismes)]
  E --> G[Verite devenue top<br/>dans les contextes pertinents]
  F --> B
```

---

## Bibliographie sélective

- J. Butterfield & C.J. Isham, *A topos perspective on the Kochen–Specker theorem: I–VI*, **Int. J. Theor. Phys.** (2000–2002).
- C.J. Isham & A. Döring, *A topos foundation for theories of physics: I–IV*, **J. Math. Phys.** (2007).
- A. Döring & C.J. Isham, *What is a Thing? Topos Theory in the Foundations of Physics*, arXiv:0803.0417 (2008).
- C. Heunen, N.P. Landsman, B. Spitters, *A topos for algebraic quantum theory*, **Commun. Math. Phys.** 291 (2009).
- A. Döring, *Topos theory and ‘neo-realist’ quantum theory*, in **New Structures for Physics**, LNP 813 (2011).
- S. Abramsky & A. Brandenburger, *The sheaf-theoretic structure of non-locality and contextuality*, **New J. Phys.** 13 (2011).
