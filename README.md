# Docker Assignment Project

This project is a machine learning web application for predicting BMW global sales using Flask and Docker. The user selects a BMW model, year, and region, then the system predicts whether the sales level is likely to be **High Sales** or **Low Sales**.

## How to Run

```bash
docker build -t bmw-app .
docker run -p 5000:5000 bmw-app

Open: http://localhost:5000

## How to Use the Website

1. Select a BMW Model from the dropdown list.

2. Select a Year from the dropdown list.

3. Select a Region from the dropdown list.

4. Press the Predict button.

5. The prediction result will be shown on the right side of the page.

## Project Structure
.
├── app.py
├── templates/
│   └── index.html
├── model.pkl
├── bmw_global_sales_2018_2025.csv
├── bmw_modified_prediction.ipynb
├── Dockerfile
├── requirements.txt
├── Demo_Assignment_Video.mp4
└── README.md

## File Descriptions

- app.py
Main Flask backend application. It loads the trained model, receives user input from the website, performs prediction, and sends the result back to the frontend.

- templates/index.html
Frontend web page of the application. It provides the user interface for selecting model, year, and region, and displays the prediction result.

- model.pkl
Saved machine learning model and encoders used for prediction in the Flask application.

- bmw_global_sales_2018_2025.csv
Dataset containing BMW global sales information used for training and analysis.

- bmw_modified_prediction.ipynb
Jupyter Notebook used for data preprocessing, model training, and exporting the final prediction model.

- Dockerfile
Docker configuration file used to build the container image for this web application.

- requirements.txt
List of Python libraries required to run the project.

- Demo_Assignment_Video.mp4
Demonstration video showing that the website runs correctly and the prediction system works as expected.

- README.md
Project documentation file containing setup steps, usage instructions, project structure, and file descriptions.

## Authors

Natthanon Narongsaksakul, st126113
https://github.com/st126113-hash/

Waranon Neamtuptim, st125934
https://github.com/Waranon021
