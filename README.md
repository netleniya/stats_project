# Flight Delay Prediction

This repository contains a machine learning model and associated code for predicting flight delays. The model is trained on historical flight data and can be used to predict whether a given flight will be delayed or not, based on various features such as airline, origin and destination airports, scheduled departure time, and more. This work is an expansion of that done as part of the final project for the Statistics for Data Science course at the University of Waterloo (2023), and adds a barebones [Streamlit](https://streamlit.io) interface for interacting with the trained model. 

## Features

- **Predictive Model**: A machine learning model trained on a large dataset of historical flight data, capable of predicting flight delays with high accuracy.
- **Data Preprocessing**: Scripts for cleaning and preprocessing raw flight data, handling missing values, and encoding categorical features.
- **Model Training**: Scripts for training the machine learning model on the preprocessed data, with options for tuning hyperparameters and selecting the best-performing model.
- **Model Evaluation**: Code for evaluating the trained model's performance on a held-out test set, including metrics such as accuracy, precision, recall, and F1-score.
- **Deployment**: Scripts and instructions for deploying the trained model as a Streamlit web service. 

## Getting Started

1. Clone the repository: `git clone https://github.com/username/flight-delay-prediction.git`
2. Preprocess the data: `python eda.py`
3. Create model pipeline: `python model.py`
4. Tune hyperparameters: `python optimizer.py`
5. Train the model: `python fit_model.py`
6. Run the model: `streamlit run main.py`

NB: The Hyperparameter tuning process can be visualized via an [Optuna](https://optuna.org) dashboard by running `optuna-dashboard sqlite:///flights.db`. 


## Contributing

Contributions are welcome! Please open an issue or submit a pull request if you have any improvements or bug fixes.

## License

This project is licensed under the [MIT License](LICENSE).

## Original project in collaboration with
- Allen, Telicia
- Dong, Lijie
- Drapinski, Michal
- Siu, Theresa
- Yang, Wenshuai

## TODO
- Organize the code better by distributing it into appropriate directories suited for CI/CD.
- Make the Streamlit app a bit less ugly.
