# Volatility Forecasting of Large Cap U.S. Equities Using GARCH Neural Network
![331shots_so](https://github.com/CalculusSlayer/ecs170_final_project_s24/assets/81405395/1a49fc1a-29b1-461e-beb6-5f18f2647ff1)

This repository contains the code and documentation for our project on forecasting the volatility of large-cap U.S. equities using a combination of Generalized Autoregressive Conditional Heteroskedasticity (GARCH) models and neural networks.

## Project Overview

The primary objective of this project is to develop a neural network model capable of forecasting the volatility of U.S. equities, specifically those that are part of the Standard and Poor's 500 index. The model utilizes GARCH techniques to capture the time-varying volatility characteristics inherent in financial data, while leveraging the powerful non-linear modeling capabilities of neural networks.

By integrating GARCH models with neural networks, we aim to improve upon the accuracy of traditional volatility forecasting methods, enabling market participants to make more informed decisions regarding portfolio management, risk management, and derivative pricing.

[ECS_170_S_24_Final_Project_Paper.pdf](https://github.com/user-attachments/files/15830598/ECS_170_S_24_Final_Project_Paper.pdf)


## Dataset

The dataset used in this project comprises hourly closing price data for all equity securities that were part of the Standard and Poor's 500 index between May 2019 and May 2024. The data was obtained from Tiingo, a financial data provider, via their Python API.

## Methodology

1. **Data Preprocessing**: The raw price data was cleaned, and any missing values were handled through backfilling or removal of securities with stock splits.

2. **Volatility Calculation**: Volatility was calculated using the logarithmic return formula, and exploratory data analysis was performed to validate the assumptions required for GARCH modeling.

3. **GARCH Model Development**: Various GARCH model variants, including standard GARCH, GJR-GARCH, and ARMA-GARCH, were implemented and optimized using gradient descent techniques.

4. **Neural Network Architecture**: An artificial neural network (ANN) architecture was designed, consisting of input, hidden, and output layers, with appropriate activation functions and optimization techniques (e.g., RMSprop, ADAM).

5. **Model Training and Optimization**: The neural network was trained using the optimized GARCH model coefficients as inputs, with the objective of forecasting future volatility.

6. **Model Evaluation**: The performance of the GARCH-neural network model was evaluated using metrics such as Root Mean Squared Error (RMSE) and compared against baseline models and alternative approaches, including Support Vector Regression (SVR) with different kernels.

## Results

The experimental results demonstrated the potential of combining GARCH models with neural networks for volatility forecasting. Specific findings and insights are detailed in the accompanying research paper.

## Usage

To run the code and reproduce the results, follow these steps:

1. Clone the repository: `git clone https://github.com/CalculusSlayer/ecs170_final_project_s24.git`
2. Install the required dependencies: `pip install -r requirements.txt`
3. Navigate to the appropriate directory and run the desired scripts or notebooks.

Please refer to the documentation within the repository for more detailed instructions and usage examples.

## Contributing

Contributions to this project are welcome. If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request.

## Authors

- Hari Suresh
- Noor-Aysha Saadat
- Mohnish Gopi
- Ashwin Chembu
- Nayeel Imtiaz
- Gautham Pandian

## License

This project is licensed under the [MIT License](LICENSE).
