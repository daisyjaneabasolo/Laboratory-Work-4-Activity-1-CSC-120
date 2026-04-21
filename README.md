# Laboratory-Work-4-Activity-1-CSC-120

https://colab.research.google.com/drive/1yGfDTP8MxJYeaEfpyh7eqdGNThinJnoV?usp=sharing

## PART 4: Compare Results (Before vs After)

| Metric              | Baseline Model (Lab 3) | Improved Model (Lab 4) |
|---------------------|------------------------|------------------------|
| Training Accuracy   | 0.9849 (98.5%)         | 0.3587 (35.9%)         |
| Validation Accuracy | 0.4810 (48.1%)         | 0.4340 (43.4%)         |
| Precision           | 0.49                   | 0.41 (Weighted Avg)    |
| Recall              | 0.48                   | 0.43 (Weighted Avg)    |
| F1-score            | 0.48                   | 0.41 (Weighted Avg)    |
| AUC Score           | 0.82                   | 0.78                   |


## GUIDE QUESTIONS (Student Explanation & Reflection)
A. Model Evaluation Analysis
1. What were the weakest-performing classes based on the confusion matrix?
2. How did Precision, Recall, and F1-score vary across classes?
3. What does a low recall indicate in your model?
4. How does AUC score reflect model performance compared to accuracy?

B. Model Improvement
5. How did data augmentation affect validation accuracy?
6. Why is Batch Normalization important in CNNs?
7. What role did Dropout play in improving your model?
8. How did Early Stopping prevent overfitting?

C. Performance Comparison
9. What improvements were observed after modifying the model?
10. Which enhancement contributed the most to performance improvement? Why?
11. Did the gap between training and validation accuracy decrease? Explain.

D. Explainability (Grad-CAM Integration)
12. How did Grad-CAM help in understanding model predictions?
13. Did the improved model focus on more relevant regions? Provide evidence.
14. Why is explainability important in real-world AI applications?
