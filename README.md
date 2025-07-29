Q1: Define overfitting and underfitting in machine learning. What are the consequences of each, and how can they be mitigated? Overfitting occurs when a machine learning model learns both the actual patterns and the noise in the training data. As a result, it performs well on the training set but poorly on new, unseen data.

Underfitting happens when the model is too simple to capture the underlying patterns in the data. It performs poorly on both the training and test sets.

Consequences:

Overfitting leads to poor generalization and low predictive accuracy on new data.

Underfitting results in inaccurate predictions because the model fails to learn enough from the training data.

Mitigation:

To reduce overfitting: use techniques like regularization, cross-validation, reducing model complexity, or gathering more training data.

To fix underfitting: increase model complexity, train for longer, or use better feature engineering.

Q2: How can we reduce overfitting? Explain in brief. Overfitting can be reduced through the following methods:

Regularization (like L1 and L2) adds a penalty to large coefficients in the model.

Cross-validation ensures the model performs well across different data splits.

Pruning (in decision trees) removes branches that add little predictive power.

Early stopping (in neural networks) halts training when performance on validation data starts to decline.

Dropout (in deep learning) randomly drops neurons during training to reduce reliance on specific features.

Simplifying the model by reducing layers, features, or nodes.

Increasing the training dataset to provide more examples and reduce the chance of memorizing.

Q3: Explain underfitting. List scenarios where underfitting can occur in ML. Underfitting happens when a model is too basic to capture the structure in the data. It doesn't perform well even on training data because it hasn’t learned the relationships properly.

Scenarios where underfitting may occur:

Using linear models on data with complex, nonlinear patterns.

Applying insufficient training time in deep learning models.

Omitting important features or poor feature engineering.

Setting a very high regularization value, which restricts the model from learning.

Choosing an oversimplified algorithm for a complex problem (e.g., using linear regression for image classification).

Q4: Explain the bias-variance tradeoff in machine learning. What is the relationship between bias and variance, and how do they affect model performance? The bias-variance tradeoff is a fundamental concept in machine learning:

Bias refers to error due to overly simplistic assumptions in the model. High bias leads to underfitting.

Variance is the error due to sensitivity to small fluctuations in the training data. High variance leads to overfitting.

Relationship:

There's a tradeoff between bias and variance. Reducing one often increases the other.

A good model finds the balance—low bias and low variance, ensuring good generalization.

Impact:

High bias → poor training and test performance.

High variance → good training but poor test performance.

Balanced → good training and test performance.

Q5: Discuss some common methods for detecting overfitting and underfitting in machine learning models. How can you determine whether your model is overfitting or underfitting? Detection Techniques:

Train vs. Test Error Comparison:

High training accuracy + low test accuracy → Overfitting

Low accuracy on both → Underfitting

Learning Curves:

Diverging curves (train ≫ test) → Overfitting

Both curves with high error → Underfitting

Cross-validation:

High variance in fold performance → Overfitting

Uniform but poor performance → Underfitting

Residual Analysis (in regression):

High, unexplained residuals → Underfitting

Structured residuals may also indicate poor generalization.

Q6: Compare and contrast bias and variance in machine learning. What are some examples of high bias and high variance models, and how do they differ in terms of their performance? Aspect High Bias High Variance Definition Model too simple to learn data Model too sensitive to training data Performance Poor on training and test sets Good on training, poor on test sets Example Linear regression on nonlinear data Deep decision tree on small dataset Result Underfitting Overfitting

Key Difference: High bias models fail to learn, while high variance models learn too much (including noise).

Q7: What is regularization in machine learning, and how can it be used to prevent overfitting? Describe some common regularization techniques and how they work. Regularization is a technique used to discourage complex models by adding a penalty term to the loss function, which prevents the model from fitting the training data too closely.

Common Techniques:

L1 Regularization (Lasso):

Adds the sum of the absolute values of coefficients to the loss.

Encourages sparsity (many weights become zero).

L2 Regularization (Ridge):

Adds the sum of squared coefficients to the loss.

Encourages smaller weights without eliminating them entirely.

Elastic Net:

Combines L1 and L2 penalties.

Useful when features are correlated.

Dropout (for neural networks):

Randomly turns off neurons during training.

Forces the network to learn redundant representations.

These methods reduce overfitting by preventing the model from becoming overly complex and memorizing the training data.
