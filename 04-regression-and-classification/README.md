# Regression & Classification

**Course:** ESE 5420, Statistics for Data Science (University of Pennsylvania, Spring 2026), Homework 8–9

**Question:** How uncertain are a regression model's predictions, and how do you train a classifier from scratch?

## What I did
- **Uncertainty in regression predictions:** derived the variance of a least-squares prediction at a new input, showed it grows with the distance from the mean of the training inputs, and built a 95% confidence interval for the mean response.
- **Logistic regression theory:** visualized the sigmoid model and the log-likelihood as 3D surfaces over the intercept and slope (NumPy and Matplotlib only), rewrote the likelihood for ±1 labels, and showed the log-likelihood is concave, so it has a single maximum.
- **Logistic regression from scratch on image data:** classified handwritten digits 0 vs. 1 (28 × 28 images) with my own NumPy implementation:
  - normalized the pixels, recoded the labels to ±1, and used a random 80/20 split, explaining why a sequential split would leave the test set unbalanced;
  - wrote the loss and gradient functions and trained with **gradient descent** for 50 epochs, plotting train and test loss and test accuracy per epoch;
  - derived the 0.5-probability decision rule.
  The model reached **90.8% test accuracy** after 50 epochs.
- **Generative classification:** derived the joint distribution for two Gaussian classes with different variances, plotted them, and explained what **linear discriminant analysis (LDA)** estimates and how it classifies.

## What I learned
- Prediction intervals widen away from the center of the data, so extrapolation deserves less trust.
- Writing the loss, gradient and training loop by hand makes clear what library classifiers do behind the scenes.
- Discriminative (logistic regression) and generative (LDA) models answer the same question from opposite directions.

## Skills and tools
Linear regression inference, prediction confidence intervals, logistic regression, maximum likelihood, concavity, gradient descent, train/test splitting, accuracy and loss curves, LDA, Gaussian class-conditional models, Python, NumPy, Matplotlib (3D plots).
