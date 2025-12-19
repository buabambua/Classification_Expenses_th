# Classification_Expenses_th
Thai Expense Classifier (NLP)
An automated expense categorization system for Thai descriptions using Machine Learning.

This project demonstrates a practical application of Natural Language Processing (NLP) to solve a common personal finance problem: automatically labeling expense transactions (e.g., "ซื้อกาแฟ" -> "Food & Beverage").

# Key Features
- Thai Language Support: Optimized for Thai text processing.
- Efficient Pipeline: Implements a Scikit-Learn pipeline combining TF-IDF Vectorization and Linear Support Vector Classification (LinearSVC).
- High Performance: Achieves high accuracy on transaction labeling.

# Tech Stack
- Python
- Pandas: For data handling and exploration.
- Scikit-learn: For the machine learning pipeline and model training.

# Model Evaluation
The model was trained on a dataset of 500 Thai expense entries and evaluated on a test set (20% split).
- Test Accuracy: 1.00 (100% accuracy on the provided sample dataset).

# Usage Example
The model can predict categories for new, unseen Thai descriptions:
# Sample Predictions
print(predict_category("กินข้าว"))               # Output: อาหาร (Food)
print(predict_category("จ่ายค่า wifi คอนโด"))    # Output: บิล/สาธารณูปโภค (Bills/Utilities)
print(predict_category("ค่าผ่อนบ้าน"))           # Output: บิล/สาธารณูปโภค (Bills/Utilities)

# Project Structure
Classification_expenses_th.ipynb: The main notebook containing the training and prediction logic.
expenses_th.csv: The dataset containing Thai expense descriptions and labels.
