


## **Problem Defination:**

The problem statement of this project is to predict the pricing range (beginner, plus, premium) of Airbnb listings in Montreal based on their attributes and descriptions. The dataset contains listings of different areas in Montreal during 2019. It comes with rich information for each listing, including a link to the thumbnails etc. The goal is to develop a multi-objective and multi-modal that combines text and image inputs to improve the accuracy of the classification. The project follows the data science life-cycle for tuning, including trying different features, hyperparameters, and modeling techniques to improve the model's performance on the public leaderboard.

---
## **Input:**

The input for the model is a combination of text and image data. The text input includes the description of the Airbnb listing, while the image input includes images of the listing.The dataset contains listings of different areas in Montreal during 2019. It comes with rich information for each listing, including a link to the thumbnails etc. These inputs are used to predict the pricing range of the listing as `beginner`, `plus`, or `premium`.

---

## **Output:**

The output of the model is a predicted pricing range category for each Airbnb listing in Montreal. The pricing range categories are `beginner`, `plus`, or `premium`, which are denoted by the labels 0, 1, and 2 respectively. The model is trained to classify each listing into one of these categories based on its input features such as description, images, location, amenities, and host information. The output of the model is a classification label denoting the predicted pricing range category for the listing.

---

## **Required Data Mining Function:**


### **Feature engineering:**
- **Extracting features from text data**: using TF-IDF.
- **Extracting features from image data**: using convolutional neural networks.

#### **Model selection and training:**

- **Convolutional Neural Network** (CNN) with image inputs.
- **Multi-Modal Deep Learning Model** that utilizes both CNN and LSTM layers to process text and image inputs.

#### **Evaluations:**

- **Calculating accuracy**: percentage of correctly classified instances.
- **Calculating precision**: percentage of true positives out of all positive predictions.
- **Calculating recall**: percentage of true positives out of all actual positives.
- **Calculating F1 score**: harmonic mean of precision and recall.

---

## **Challenges**

- **Ensuring data quality**, dealing with missing data, outliers, and ensuring representative data.

- **Diffrent languages**: the text column contains text different languageColumns (or Features) that contain text with different language.

- **Images size**: Dealing with images in diffrent sizesDealing with images in diffrent sizes.

- **Multi-modality**, combining different types of inputs in a single model.

- **Overfitting**, preventing the model from fitting noise in the training data.

- **Model complexity**, selecting the appropriate architecture and hyperparameters.

- **Interpretability**, understanding the model's predictions and important features.


Addressing these challenges requires careful consideration of the data, model architecture, and hyperparameters, as well as the use of appropriate evaluation metrics and techniques for model interpretation and explanation.

---
## **Impact**


Building a machine learning model for predicting the pricing range category of Airbnb listings in Montreal can have several impacts, including:

- **Improved user experience**: By providing accurate pricing recommendations to new hosts, the model can help ensure that guests are getting fair and competitive prices for their Airbnb stays. This can lead to improved user satisfaction and repeat business.

- **Increased revenue for hosts**: By recommending pricing ranges that are appropriate for the listing, hosts can avoid underpricing their listings and missing out on potential revenue. This can help hosts maximize their earnings from their Airbnb listings.

- **Improved market insights**: By analyzing the features and attributes of successful listings, the model can provide insights into what makes a successful Airbnb listing in Montreal. This information can be valuable for the tourism industry and other stakeholders.

- **Increased efficiency**: By automating the pricing recommendation process, the model can save hosts time and effort in setting prices for their listings. This can lead to increased efficiency and productivity for hosts.

- **Improved pricing**: By leveraging machine learning algorithms, the model can provide more accurate pricing recommendations than traditional manual methods. This can lead to improved pricing and more competitive listings.

Overall, the impact of building a machine learning model for predicting the pricing range category of Airbnb listings in Montreal can be significant, benefiting hosts, guests, and the tourism industry as a whole.

---

## **Ideal Solution:**

- Best accuracy in leaderboard is 0.62934. It is produced by LSTM and CNN (model3) without using transfer learning.
- I traied RGB images but it doesn't improve the accuracy.
- I traied 'sgd' optimizer with the simple model (model1), but the accuracy decresed on leaderboard sharply (0.4682)
- Simple RNN didn't produce bad performance.

---



