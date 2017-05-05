#Linear Regression
from sklearn.linear_model import LinearRegression
lr = LinearRegression()
lr.fit(cars[["weight"]], cars["mpg"])
predictions = lr.predict(cars[["weight"]])
from sklearn.metrics import mean_squared_error
mse=mean_squared_error(predictions,cars["mpg"])
mse
