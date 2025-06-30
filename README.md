**📊 Energy Consumption Forecasting**

**Project Overview**

This project is about building a time-series forecasting model to predict hourly energy consumption using the PJME Hourly dataset.

I started by exploring a simple linear regression model, then moved to ARIMA, and finally tested a SARIMA model to see if adding seasonality would improve forecasting accuracy.

The idea was to compare different models and see which one works better for this type of energy data.


**What I Did**

📌 Cleaned and prepared the dataset

📌 Built a simple linear regression model to check the general trend

📌 Developed an ARIMA model to handle time-based patterns

📌 Improved the model using SARIMA to account for seasonality

📌 Compared the results using MAE and MSE

📌 Visualized all the models to check how close they are to the actual data


**Model Comparison**
**Model**								**MAE**	            **MSE**

Linear Regression	    5,275.51 MW	    43,203,776.13

ARIMA (1, 0, 1)	      5,331.82 MW	    43,633,423.47

SARIMA	              5,287.31 MW	    37,107,301.01

The SARIMA model provided the best balance because it handled seasonality better and gave the lowest MSE.

**Key Takeaways**
- Linear models can sometimes predict surprisingly well, especially when the data follows a strong trend.
- ARIMA needs to be carefully tuned, and without seasonality, it might not perform well.
SARIMA is a solid option when the data clearly shows seasonal patterns.

**Tools I Used**
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Statsmodels
- scikit-learn
- Jupyter Notebook
  
**Next Steps**
- Try more advanced seasonal tuning for SARIMA
- Test weekly seasonality patterns
- Explore building an LSTM model using TensorFlow
- Try developing a simple dashboard to visualize forecasts better

**About Me**
I’m exploring computational energy systems and applying machine learning to energy challenges. This is one of my first projects on this journey.
