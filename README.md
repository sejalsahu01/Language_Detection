## Language detection model using Machine Learning (ML) and Natural Language Processing (NLP)
### **Project Description**
This project is a simple language detection system that uses Machine Learning and Natural Language Processing (NLP) techniques. It predicts the language of a given input text based on trained data.

---
### **Features**
- Detects languages based on text input.
- Supports multiple languages.
- Built with Scikit-learn, CountVectorizer, and MultinomialNB.
- Easy to use and efficient for classification tasks.

---
### **Installation**
1. Clone this repository:
```bash
git clone https://github.com/sejalsahu01/Language_Detection
cd Language_Detection
```
2. Install required dependencies:
 ```bash
 pip install -r requirements.txt
 ```
3. Run the Jupyter Notebook to explore or modify the model:
 ```bash
 jupyter notebook
 ```
---
### **How It Works**
1. Data preprocessing:
   - Convert text into numerical data using ```CountVectorizer```(Bag-of-Words approach).
   - Train the model using ```MultinomialNB```.
2. Model Training:
   - Use the text dataset to train the Naive Bayes model.
3. Prediction:
   - Input a sentence, and the model predicts the language.
---
### **Code Example**
```bash
# Input text from the user
user = input("Enter a text ")

# Transform input into numerical data
data = cv.transform([user]).toarray()

# Predict the language
output = model.predict(data)

# Display the result
print("Predicted Language:", output)

```
--- 
### **File Structure**
```bash
Language_Detection/
├── Language_Detection.ipynb  # Main notebook for training and testing
├── README.md                 # Project documentation
├── requirements.txt          # List of dependencies
└── data/                     # Dataset used for training

```
---
### **Libraries Used**
- Pyhon 3.x
- Scikit-learn
- NumPy
- Pandas
- Jupyter Notebook
---
### **Usage**
1. Run the notebook:
```bash
jupyter notebook Language_Detection.ipynb
```
2. Enter a sentence when prompted, and the system will detect the language.
---
### **Example Output**
```bash
Enter a text :  ใน พศ หลักจากที่เสด็จประพาสแหลมมลายู ชวา อินเ
Predicted Language: ['Thai']
```
---
### **Future Improvements**
- Add support for more languages.
- Improve accuracy with larger datasets.
- Implement deep learning-based for better results.
---
### **Contributions**
Feel free to fork the repository and submit pull requests for improvements! 😊
