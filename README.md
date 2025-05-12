# Machine Learning Sentiment Analysis with ML.NET

This is a C# machine learning project that uses **ML.NET** to perform **sentiment analysis** on a dataset of Yelp reviews. The model is trained to classify reviews as either **positive** or **negative** based on their text content. The project uses **Logistic Regression** for binary classification and evaluates the model's performance with metrics like Accuracy, AUC, and F1-Score.

## Features
- Load and preprocess a dataset of labeled reviews (`yelp_labelled.txt`).
- Build and train a sentiment classification model using **ML.NET**.
- Evaluate the model's accuracy using **Accuracy**, **AUC**, and **F1-Score**.
- Interactive CLI where users can input text and receive a sentiment prediction.

---

## Prerequisites

Before you can run this project, make sure you have the following tools installed:

- **.NET SDK 7.0** or later: [Download .NET SDK](https://dotnet.microsoft.com/download)
- **Visual Studio Code** (VS Code): [Download Visual Studio Code](https://code.visualstudio.com)
- **C# Dev Kit Extension** for Visual Studio Code: [Install C# Extension](https://marketplace.visualstudio.com/items?itemName=ms-dotnettools.csharp)

---

## Getting Started

Follow these steps to get the project up and running on your local machine:

### 1. Clone the Repository

Clone the project repository to your local machine using the following command:

```bash
git clone https://github.com/vignesh0801-beep/MachineLearningDotnet7.git
cd MachineLearningDotnet7
2. Open the Project in Visual Studio Code
Open the project folder in VS Code:

bash
Copy
Edit
code .
If you're using Visual Studio Code, you'll be prompted to add required assets like launch.json and tasks.json — click Yes to enable debugging.

3. Restore Dependencies
Ensure all the dependencies are installed by running the following command in the terminal:

bash
Copy
Edit
dotnet restore
4. Add the Dataset
Make sure the yelp_labelled.txt file exists in the MachineLearning directory. The dataset should be in tab-separated format with review text and sentiment labels.

Running the Project
Once you've set everything up, you can run the project using the following command:

bash
Copy
Edit
dotnet run --project MachineLearning
This will train the model, evaluate its accuracy, and then enter an interactive loop where you can input text and get a sentiment prediction.

Sample Interaction:
text
Copy
Edit
What's your [green]review text[/]?
> The food was amazing!

👍 [green]"The food was amazing!" (99%) 

What's your [green]review text[/]?
> Terrible experience, would never go back.

👎 [red]"Terrible experience, would never go back." (92%)
How It Works
Data Loading: The project loads the dataset yelp_labelled.txt, which contains text reviews and their sentiment labels (positive/negative).

Model Training: It uses Logistic Regression as the classification model.

Evaluation: After training, the model is evaluated on a test set, and key metrics like Accuracy, AUC (Area Under the Curve), and F1-Score are displayed.

Interactive Prediction: Users can input a review, and the model will predict if the sentiment is positive or negative.

