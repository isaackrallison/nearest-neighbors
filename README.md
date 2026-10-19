# Nearest Neighbor Lab

An interactive study guide for §16.1 and §16.2.2–16.2.4 of Kevin P. Murphy, *Probabilistic Machine Learning: An Introduction*
(K nearest neighbor classification; deep metric learning, classification losses and ranking losses). §16.2.1 (LMNN, NCA, LCA) is not covered.

**Live:** https://isaackrallison.github.io/nearest-neighbors/

Every section has an **Explain it** box at four levels (Kid, High school, Undergrad, Grad / MLE), switchable globally from the top bar.

- **16.1 KNN classification:** drag a test point through three classes, change K, and switch from Euclidean to a Mahalanobis distance with adjustable weights and rotation. The neighborhood outline becomes an ellipse. Eq. 16.1 bars, neighbor table, optional prediction shading.
- **16.1.1 Example:** an editable Voronoi diagram with exact cells (Figure 16.1b), and decision regions with train/test error for K = 1…80 (Figure 16.2).
- **16.1.2 Curse of dimensionality:** e_D(p) = p^(1/D) curves with per-axis coverage bars (Figure 16.3), plus a distance-concentration histogram for D up to 200.
- **16.1.3 Speed and memory:** a k-d tree search that counts distance computations, a k-d tree vs dimension experiment, and random-line LSH with bucket shading and recall.
- **16.1.4 Open set recognition:** a face gallery with a match threshold, "enroll as new person", and false accept / false reject curves.
- **16.2.2 Deep metric learning:** drag two embeddings and check Eq. 16.9 (normalized distance = 2 − 2·cosine).
- **16.2.3 Classification losses:** two embeddings with the same linear accuracy and different 1-NN accuracy.
- **16.2.4.1–16.2.4.3 Ranking losses:** contrastive loss curves and a Siamese diagram; a triplet playground with easy / semi-hard / hard regions and gradient steps; an N-pairs lineup on the unit circle with temperature, and logistic vs hinge (Eqs. 16.14–16.15).
- **Compare:** train a free-parameter embedding live with each of the three losses.
- Step-by-step math for Eqs. 16.1–16.2 and 16.7–16.15, a 55-question quiz tagged by level, and a cheat sheet.

Single self-contained `index.html`, no build step. Loads Google Fonts and MathJax from cdnjs. All data are synthetic and generated in the page from fixed seeds.
