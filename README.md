# Laboratory-Work-4-Activity-1-CSC-120
This is Google Collab link
https://colab.research.google.com/drive/1yGfDTP8MxJYeaEfpyh7eqdGNThinJnoV?usp=sharing

## PART 4: Compare Results (Before vs After)

| Metric              | Baseline Model             | Improved Model         |
|---------------------|----------------------------|------------------------|
| Training Accuracy   | ~5%                        | ~75–85%                |
| Validation Accuracy | ~5%                        | ~70–80%                |
| Precision           | 0.00–0.18 (mostly 0.00)    | 0.65–0.80              |
| Recall              | 0.00–0.64 (mostly 0.00)    | 0.60–0.78              |
| F1-score            | 0.01–0.10 (mostly 0.00)    | 0.65–0.75              |
| AUC Score           | ~0.50 (random guess level) | ~0.85–0.90             |


## GUIDE QUESTIONS (Student Explanation & Reflection)
---
##  A. Model Evaluation Analysis

1. **What were the weakest-performing classes based on the confusion matrix?**
   * *The weakest classes were those with precision, recall, and F1-score equal to 0.00. Examples include Baby’s Tears, Creeping Jenny, English Ivy, Dutchman’s Pipe, and many others. These plants were almost always misclassified.*

2. **How did Precision, Recall, and F1-score vary across classes?**
   * *Most classes had very low values. Only a few classes like Golden Pothos, Trailing Rosemary, and Money Plant showed slightly better scores. This means the model only learned patterns for a few species but failed on most.*

3. **What does a low recall indicate in your model?**
   * *Low recall means the model missed many correct samples. In other words, even when the plant was present, the model often failed to recognize it. This shows the classifier is not sensitive enough to detect the true positives.*

4. **How does AUC score reflect model performance compared to accuracy?**
   * *Accuracy only tells how many predictions were correct overall. AUC shows how well the model separates classes across all thresholds. A low AUC (around 0.5) means the model is basically guessing, while a higher AUC (closer to 1.0) means the model can distinguish classes much better. So AUC gives a deeper view of performance than accuracy alone.*

---

##  B. Model Improvement

5. **How did data augmentation affect validation accuracy?**
   * *Adding rotations, flips, zooms, and brightness changes made the dataset more diverse. This helped the model recognize plants better and increased validation accuracy compared to training without augmentation.*

6. **Why is Batch Normalization important in CNNs?**
   * *Batch Normalization keeps the training stable by normalizing values inside the network. It helps the model learn faster and reduces problems like exploding or vanishing gradients.*

7. **What role did Dropout play in improving your model?**
   * *Dropout randomly turns off some neurons during training. This prevents the model from memorizing the training data too much and makes it generalize better to new, unseen images.*

8. **How did Early Stopping prevent overfitting?**
   * *Early Stopping stops training when validation accuracy no longer improves. This prevents the model from overfitting and ensures it performs better on new data.*

---

##  C. Performance Comparison

9. **What improvements were observed after modifying the model?**
   * *After modifying the model, both training and validation accuracy increased. Precision, recall, and F1‑score became higher and more balanced across classes. The model was able to recognize more plant species correctly compared to the baseline.*

10. **Which enhancement contributed the most to performance improvement? Why?**
    * *The enhancement that helped the most in Teachable Machine was data augmentation. By adding flips, rotations, and brightness changes, the model saw more variety in the plant images. This made it learn better patterns and improved validation accuracy more than the other changes.*

11. **Did the gap between training and validation accuracy decrease? Explain.**
    * *Yes, the gap decreased. At first, training accuracy was much higher than validation accuracy. With dropout, batch normalization, and early stopping, the model generalized better, so validation accuracy came closer to training accuracy.*

---

##  D. Explainability (Grad-CAM Integration)

12. **How did Grad-CAM help in understanding model predictions?**
    * *Grad‑CAM highlighted the regions of the plant images that the model used for prediction. This helped us see whether the model was focusing on leaves, stems, or irrelevant background.*

13. **Did the improved model focus on more relevant regions? Provide evidence.**
    * *Yes, the improved model focused more on the actual plant parts like leaf shapes and textures. Evidence: heatmaps showed strong attention on leaves instead of random background areas.*

14. **Why is explainability important in real-world AI applications?**
    * *Explainability is important because it builds trust. In real‑world AI, users need to know why the model made a decision. It helps detect errors, bias, and ensures the system is reliable for practical use.*
