# Sentimental-Analysis-of-Drug-Review-Dataset

Comparison between results given by TextBlob and Logistic Regression

To Download dataset click [here](https://www.kaggle.com/jessicali9530/kuc-hackathon-winter-2018)

---

### Requirements
- NumPy
- Pandas
- Matplotlib
- Seaborn
- scikit-learn
- Regex
- [TextBlob](https://textblob.readthedocs.io/en/dev/)
- Word Cloud
- Warnings
- NLTK
---

### Import Dataset
   - Both train and test dataset
 
![Capture](https://user-images.githubusercontent.com/79501547/140917480-a5c078ed-e9de-44c3-b491-5ffc74f3e62d.PNG)

### Size of the dataset
![tempsnip](https://user-images.githubusercontent.com/79501547/140917586-3c2be06b-9a00-41a9-b0be-531a5b58427f.png)

### Visualization
![Capture](https://user-images.githubusercontent.com/79501547/140918019-ee285f6e-61f4-491b-bbc8-f954181df23b.PNG)

### Uniqueness of the datasets
![Capture](https://user-images.githubusercontent.com/79501547/140918233-205c4b37-7288-488d-9384-b4f2d491fa45.PNG)

### Preprocessing of the data
![Capture](https://user-images.githubusercontent.com/79501547/140918697-d61a196b-5da3-4e36-bc99-45a343ad0531.PNG)

`review_clean` function take raw text as input and return clean text as output.

### Word Cloud of Positive Reviews
![Capture](https://user-images.githubusercontent.com/79501547/140919226-80d04a74-94ae-4219-8123-544509336d6a.PNG)

### Word Cloud of Negative Reviews
![Capture](https://user-images.githubusercontent.com/79501547/140919354-eee4f337-05ea-49ad-8e68-47d984f0a69e.PNG)


### Word Cloud of Neutral Reviews
![Capture](https://user-images.githubusercontent.com/79501547/140919435-3de52d84-e6fe-46bf-8860-43b53722ce0a.PNG)

## TextBlob
The sentiment property returns a named tuple of the form Sentiment(polarity, subjectivity). The polarity score is a float within the range [-1.0, 1.0]. The subjectivity is a float within the range [0.0, 1.0] where 0.0 is very objective and 1.0 is very subjective.

> After getting polarity from TextBlob and processing in to (-1, 0, 1) as feature named analysis

![Capture](https://user-images.githubusercontent.com/79501547/140920147-a60b7745-32a8-48ba-9b85-fd1e53d4ef41.PNG)
---

Applying same technique on test dataset

***Alognside this, we train Logistic Regression model on train_dataset***

### Comparison between TextBlob and Logistic Regression
![Capture](https://user-images.githubusercontent.com/79501547/140921087-d401ad20-a2c5-47cc-b26e-0e136b02498a.PNG)

> Result

```
Final Accuracy by training Logistic Regression model is : 0.8902769725645677
Final Accuracy of TextBlob on test set is: 0.5959866095640628
```
