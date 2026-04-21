# LW4_Improving-CNN-Performance
## Google Colab link: https://colab.research.google.com/drive/1O74Hp2zpO2kT_qQRaYWCc5G_eIJilSpG?usp=sharing

## 🧠 A. Model Evaluation Analysis

1. What were the weakest-performing classes based on the confusion matrix?
The weakest-performing classes were those with the highest misclassification rates in the confusion matrix. These classes had many incorrect predictions, often being confused with similar-looking classes.

2. How did Precision, Recall, and F1-score vary across classes?
Precision, Recall, and F1-score varied depending on how well each class was learned by the model. Some classes had high precision and recall (well-classified), while others had lower values, indicating difficulty in distinguishing those classes.

3. What does a low recall indicate in your model?
A low recall indicates that the model is failing to correctly identify many actual instances of a class (high false negatives). This means the model is missing important predictions.

4. How does AUC score reflect model performance compared to accuracy?
AUC provides a more comprehensive evaluation than accuracy because it measures how well the model distinguishes between classes across all thresholds, while accuracy only measures overall correctness.

## ⚙️ B. Model Improvement

5. How did data augmentation affect validation accuracy?
Data augmentation improved validation accuracy by increasing dataset diversity, allowing the model to generalize better and reducing overfitting.

6. Why is Batch Normalization important in CNNs?
Batch Normalization stabilizes and speeds up training by normalizing layer inputs, which helps improve convergence and overall model performance.

7. What role did Dropout play in improving your model?
Dropout reduced overfitting by randomly disabling neurons during training, forcing the model to learn more robust and generalized features.

8. How did Early Stopping prevent overfitting?
Early Stopping monitored validation loss and stopped training once performance stopped improving, preventing the model from memorizing the training data.

## 📊 C. Performance Comparison

9. What improvements were observed after modifying the model?
After modification, the model showed higher validation accuracy, lower validation loss, improved F1-scores, and better generalization.

10. Which enhancement contributed the most to performance improvement? Why?
Data augmentation contributed the most because it exposed the model to more diverse training samples, significantly improving generalization.

(Alternative answer: Dropout or BatchNorm — depends on your results)

11. Did the gap between training and validation accuracy decrease? Explain.
Yes, the gap decreased, indicating reduced overfitting and improved generalization. The model performed more consistently on both training and validation data.

## 🔍 D. Explainability (Grad-CAM Integration)

12. How did Grad-CAM help in understanding model predictions?
Grad-CAM highlighted the important regions in the image that influenced the model’s decision, making it easier to understand how predictions were made.

13. Did the improved model focus on more relevant regions? Provide evidence.
Yes, the improved model focused more on relevant object areas rather than background regions, as shown by clearer and more concentrated heatmaps.

14. Why is explainability important in real-world AI applications?
Explainability builds trust, helps detect errors or bias, and ensures that AI decisions are reliable and interpretable, especially in critical applications like healthcare and finance.
