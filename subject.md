# ZOIDBERG2.0

Given some X-ray images, use machine learning to help doctors detecting pneumonia.

Doctors granted you access to 3 datasets.

> [!NOTE]
> It's up to you to decide when and how to use the dataset (training, testing, evaluating performance, tuning parameters, ...).

You must:
* use a train-validation-test procedure,
* use a cross validation procedure,
* compare your results with a simple train test split,
* use one of the datasets to tune your algorithms.

You MUST explore and test various methods, **and to compare results**.

> [!NOTE]
> optimization, feature engineering, metrics, PCA

> [!IMPORTANT]
> A clear and concise way to present results should always prevail.

## Delivery

You are expected to deliver:

* Technical documents
    a **Jupyter notebook-like file**, containing code and text, possibly graphics and an html-file to prove your results without rerunning the code
* a synthesis document
    a pdf file to sum up your results and figures

### Notebook structure requirements

Your Jupyter notebook must include the following:

1. **Introduction**
   - A clear description of the problem: what you are doing and why.
   - A list of all requirements and dependencies (libraries, dataset, environment).

2. **Research questions**
   Define exactly **three questions** in a clear and explicit manner, then answer each one. Examples:
   - *"Can we achieve 99% accuracy?"* (the answer is almost certainly no — explain why)
   - Frame your questions around what insights or limitations you want to explore.

3. **Preprocessing explanation**
   Document the full preprocessing pipeline:
   - Image conversion (e.g., grayscale, resizing)
   - Normalization / standardization
   - Any augmentation, feature extraction, or dimensionality reduction steps

4. **Algorithms**
   Implement and compare **at least three different algorithms**.
   - Justify your choice of algorithms.
   - Explain why some perform better than others on this dataset.

5. **Results and visualizations**
   Every result must be accompanied by:
   - A **diagram** or plot
   - A **title** and a **legend**
   - Comments explaining what the result shows

6. **Saving trained models**
   Training results must be saved to disk (e.g., using `joblib`, `pickle`, or framework-specific formats) so the notebook can be re-run and load pre-trained models without retraining from scratch.

> [!NOTE]
> There are ways to save a trained algorithm and load it afterwards in order to obtain the same results when you run it again!

## Bonus

You can improve your project in many ways, including:

* implementing a self-organizing map to help you visualize your result,
* thorough learning through neural networks,
* predicting on 3 classes: no pneumonia, virus pneumonia, bacteria pneumonia,

## Recommendations

### Time and space

Think carefully about needed resources (such as the complexity, for execution and for storage) **before** starting implementation. For quicker or better results, you may _— or may not —_ want to transform your data.

> [!NOTE]
> Some libraries could help you.

### Bad habits

Do not let your algorithm(s) make bad habits. Find the correct balance between **bias** and **variance**. Cross validation procedures can help you solve this problem. It's also a good idea when you don't have a lot of data.

Algorithms' parameters can also help you to find a trade-off between bias and variance, this is why you need a good understanding on how they work.

### Good metrics

Find an explicit way to show your results, in a readable way.
You must choose among many various metrics and **select the appropriate one(s)**.

Look at more advanced metrics like ROC-AUC score.
It will give you a deeper understanding of your results.
You should also be able to explain what AUC measures and its advantages over other metrics.

> [!NOTE]
> First ML project!? You should dig a bit and find answers: the only way out is the way in!
