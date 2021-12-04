Machine Learning Algorithm with SVM and Linear Regression

A) You have to get your own API from :
data.nazdaq.com
and apply that at the beginning of the code:
quandl.ApiConfig.api_key = "V8TNZ9p-k2fXDf1Wqw7T"

B) If you want to use SVM instead of LinearRegression in the current code, just do the following:
use
clf = svm.SVR(kernel='poly')
with any kernel you want (Linear,...)
instead of
clf = LinearRegression(n_jobs=-1)
in the code

C) you can substitude WIKI/GOOGL in:
df = quandl.get('WIKI/GOOGL')
with any stock you want, but remember that you have to change the codes
