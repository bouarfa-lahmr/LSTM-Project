# 📈 Stock Price Prediction using LSTM Neural Networks

A deep learning project that predicts stock prices using Long Short-Term Memory (LSTM) neural networks. This project analyzes historical stock data from 19 major technology companies and builds predictive models to forecast future closing prices.

## 🎯 Project Overview

This project explores the application of LSTM neural networks for financial time series prediction. By leveraging the temporal dependencies in stock price data, the model can learn complex patterns and make accurate predictions about future price movements.

### Key Features

- **Multi-Stock Analysis**: Analyzes 19 major tech companies (AMZN, META, NFLX, AAPL, GOOGL, MSFT, etc.)
- **Advanced Deep Learning**: Implements LSTM architecture optimized for time series prediction
- **Comprehensive Data Pipeline**: Automated data collection, preprocessing, and normalization
- **Performance Evaluation**: Detailed analysis with MSE metrics and visualization
- **Robust Training**: Includes early stopping and dropout layers to prevent overfitting

## 🛠️ Technologies Used

- **Python 3.8+**
- **TensorFlow/Keras** - Deep learning framework
- **yfinance** - Yahoo Finance data extraction
- **scikit-learn** - Data preprocessing and scaling
- **pandas** - Data manipulation and analysis
- **numpy** - Numerical computations
- **matplotlib/seaborn** - Data visualization

## 📊 Dataset

- **Source**: Yahoo Finance via yfinance library
- **Period**: January 1, 2010 - January 1, 2024
- **Companies**: 19 major technology stocks
- **Features**: Focus on closing prices for prediction
- **Data Split**: 80% training, 20% testing

### Companies Analyzed
Amazon (AMZN), Meta (META), Netflix (NFLX), Apple (AAPL), Google (GOOGL), Microsoft (MSFT), and 13 other major tech companies.


### Advanced Configuration

Modify the configuration in `config.py`:
- Adjust sequence length (default: 60 days)
- Change model architecture parameters
- Set training epochs and batch size
- 
## 📈 Model Architecture

- **Input Layer**: 60-day sequence of closing prices
- **LSTM Layers**: Two stacked LSTM layers with dropout
- **Output Layer**: Single dense layer for price prediction
- **Optimization**: Adam optimizer with MSE loss function
- **Regularization**: Dropout layers and early stopping

### Training Details
- **Epochs**: 50 (with early stopping)
- **Batch Size**: 32
- **Validation Split**: 20%
- **Sequence Length**: 60 days
- **Normalization**: MinMaxScaler (0-1 range)

## 📊 Results

The LSTM model demonstrates strong performance across multiple metrics:

- **Training Accuracy**: High correlation between predicted and actual prices
- **Test Performance**: Good generalization with low MSE values
- **Visual Analysis**: Close alignment between predicted and actual price curves
- **Temporal Consistency**: Maintains chronological data integrity

### Performance Metrics
- Mean Squared Error (MSE) calculated for both training and test sets
- Visual comparison charts for each stock
- Convergence analysis of training and validation loss

## 🔬 Key Findings

1. **LSTM Effectiveness**: Successfully captures temporal dependencies in stock price data
2. **Preprocessing Impact**: Proper normalization and sequence creation crucial for performance
3. **Generalization**: Model performs well on unseen test data
4. **Market Volatility**: Predictions remain sensitive to inherent market complexity


## 👨‍💼 Author

**BOUARFA LAHMAR**
- Supervised by: M. K.ELMOUTAOUAKIL

## 📚 Documentation

For detailed technical documentation and analysis (in French), please refer to:

**[📋 Click here to see project report (French version)](link-to-your-french-report)**

## 🙏 Acknowledgments

- Yahoo Finance for providing accessible financial data
- TensorFlow team for the excellent deep learning framework
- The open-source community for valuable libraries and tools

