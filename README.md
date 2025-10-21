# Turkish Text Classification with NLTK and Zemberek

This project implements a Turkish natural language classification pipeline using NLTK, Zemberek, and scikit-learn classifiers.
It includes the following features:
- Reads labeled Turkish sentences from an Excel dataset
- Preprocesses and normalizes the text using Zemberek and TurkishStemmer
- Extracts word stems and removes Turkish stopwords
- Trains multiple classifiers including:
   * Naive Bayes
   * MultinomialNB
   * BernoulliNB
   * Logistic Regression
   * SGDClassifier
   * LinearSVC
- Combines multiple classifiers into an ensemble (Voting Classifier) for a better accuracy.

## Example Usage

```python
ex_data = "drone'lar bugün çizgi olacaksınız"
print(f"Classification: {voted_classifier.classify(find_features(ex_data))}")
print(f"Confidence %: {voted_classifier.confidence(find_features(ex_data))*100}")
```

**Output:**

```
Classification: Çizgi
Confidence %: 100.0
```
---

## 📄 License

This project is released under the **MIT License**.
You may use, modify, and distribute it freely for educational or research purposes.
