# Model Selection, Clustering & PCA

**Course:** ESE 5420, Statistics for Data Science (University of Pennsylvania, Spring 2026), Homework 10–11

**Question:** How do you choose model complexity without overfitting, and how do you find structure in data without labels?

## What I did
- **Polynomial regression with cross-validation:** fit polynomial models of degree 1 to 40 and used **5-fold cross-validation** (scikit-learn) to compare their mean squared error. The CV curve picked a **degree-3** polynomial, which I then fit to the full dataset and plotted against the data.
- **k-means by hand and in code:** clustered 16 points arranged in a cross shape, starting from four given corner centers. I traced the assignments and centroid updates step by step and showed that this start converges to quadrant-based clusters, a **local minimum**, instead of the optimal four-arm clustering.
- **PCA fundamentals:** found principal components by inspection and by computation, showed how **standardizing** the data changes the components (PCA isn't scale invariant), and projected data onto the first component.
- **Eigenfaces:** ran **randomized PCA** on the Labeled Faces in the Wild image dataset to extract 150 components, displayed the top 25 "eigenfaces", and reconstructed faces from the 150 components. The reconstructions kept each face's overall structure and lost fine detail and texture.

## What I learned
- Cross-validation turns "how complex should the model be?" into a measurable choice.
- k-means depends on its starting point, so multiple restarts or better initialization matter.
- PCA compresses data into its main directions of variation, but you have to decide whether to standardize first.

## Skills and tools
Polynomial regression, k-fold cross-validation, bias-variance trade-off, k-means clustering, PCA, randomized PCA, standardization, dimensionality reduction, image data, Python, scikit-learn, pandas, NumPy, Matplotlib, Seaborn.
