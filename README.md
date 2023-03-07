# PROJECT ECONOMIC BUSINESS INSIGHTS FROM AFRICAN CRISIS DATASET




**General Description**

DATASET

This dataset is a derivative of Reinhart et al.'s Global Financial Stability dataset, which can be found online at: https://www.hbs.edu/behavioral-finance-and-financial-stability/data/Pages/global.aspx

It specifically focuses on the Banking, Debt, Financial, Inflation and Systemic Crises that occurred, from 1860 to 2014, in 13 African countries, including: Algeria, Angola, Central African Republic, Ivory Coast, Egypt, Kenya, Mauritius, Morocco, Nigeria, South Africa, Tunisia, Zambia and Zimbabwe.

The dataset will be valuable to those seeking to understand financial stability dynamics within the African context.

The columns in the dataset include the following:

- case: A unique identifier for each country.
- cc3: A three-letter country code.
- country: The name of the country.
- year: The year for which the economic indicators are reported.
- systemic\_crisis: A binary indicator of whether the country had a systemic crisis in that year.
- exch\_usd: The exchange rate of the country's currency to the US dollar.
- domestic\_debt\_in\_default: A binary indicator of whether the country's domestic debt was in default.
- sovereign\_external\_debt\_default: A binary indicator of whether the country's external debt was in default.
- gdp\_weighted\_default: A binary indicator of whether the country's default was weighted by its GDP.
- inflation\_annual\_cpi: The annual inflation rate of the country's consumer price index (CPI).
- independence: A binary indicator of whether the country was independent in that year.
- currency\_crises: A binary indicator of whether there was a currency crisis in the country in that year.
- inflation\_crises: A binary indicator of whether there was an inflation crisis in the country in that year.
- banking\_crisis: A categorical variable indicating whether there was a banking crisis in the country in that year, with possible values "crisis" and "no\_crisis".

PROJECT

Data cleaning : 

- first we are going to drop some columns
- change data type values in banking\_crises column to 0s and 1s
- In currency\_crises column there is 4 rows its value is 2 but this is error because this column must include 0s and 1s

Data Explorations

- Heatmap
- Lineplot
- Subplots
- Scatterplot

Data Analysis 

- function visual\_summary : Function creates different types of visualizations (histogram, scatter plot, pie chart) based on the input type\_, the input DataFrame df, and the input column col.
- function central\_tendency : This function calculates the central tendency (mean, median, mode)  of the values in a specified column of a pandas DataFrame based on the input type\_.
- Function measure\_of\_dispersion : The function takes three arguments: type\_ which specifies the type of the measure of dispersion to be calculated (e.g. range, MAD, std dev, CV, iqr, or cov), df which is the DataFrame, and col which is the column name for which the dispersion measure is to be calculated.
- Function calculate\_correlation() : Calculates either Pearson or Spearman correlation coefficient between two columns of a pandas DataFrame. It creates a new DataFrame by selecting only the specified columns and then calculates the correlation coefficient using the appropriate formula depending on the specified correlation type. Finally, the function returns the calculated correlation coefficient or prints a message if the specified correlation type is invalid.
- Function calculate\_probability\_discrete : Calculates the total number of observations in the dataset using the value\_counts method on data followed by the sum method. It then calculates the number of occurrences of the specific event in the dataset using the value\_counts method on data and indexing with event.
- Function event\_independence\_check : Checks if two events, represented by their individual probabilities prob\_event1 and prob\_event2 and their joint probability prob\_event1\_event2, are independent or not.
- Function bayes\_theorem : Calculates the conditional probability of an event, given the occurrence of another event, using Bayes' theorem. The function takes five parameters: df, which is the input pandas DataFrame, col1 and col2, which are the names of two columns in the DataFrame, event1 and event2, which are the specific events whose probabilities are to be calculated.
- Various measures of dispersion can be calculated for different variables in a pandas DataFrame using the measure\_of\_dispersion() function. These measures provide insights into the distribution of the data and can be used to make informed decisions and draw conclusions about the dataset. By calculating the range, MAD, CV, standard deviation, and covariance of different variables, we can better understand the spread and variability of the data. 
- insights into the likelihood of banking crises occurring in different countries. We can use this information to make informed decisions and take preventive measures to avoid financial crises in the future.
- The conditional probability of inflation crisis given banking crisis is calculated. Then, the independence between banking crisis and inflation crisis is checked using the previously defined function. Later, the probability of banking crisis given that other crises (systemic, currency, and inflation crises) have already occurred is calculated using Bayes theorem. The final output is the probability of banking crisis given other crises have already occurred. The conclusion could be that the probability of banking crisis increases if other crises have already occurred.

**Installation Requirements** 

1. Python - You need to have Python installed on your system to run the IPYNB file. You can download Python from the official website: https://www.python.org/downloads/.

1. Jupyter Notebook - IPYNB files are Jupyter Notebook files. You need to have Jupyter Notebook installed on your system to open and run the IPYNB file. You can install Jupyter Notebook using pip command: pip install jupyter.

1. NumPy - NumPy is a Python library used for numerical computing. You need to have NumPy installed on your system to use it in the IPYNB file. You can install NumPy using pip command: pip install numpy.

1. Pandas - Pandas is a Python library used for data manipulation and analysis. You need to have Pandas installed on your system to use it in the IPYNB file. You can install Pandas using pip command: pip install pandas.

1. Matplotlib - Matplotlib is a Python library used for data visualization. You need to have Matplotlib installed on your system to use it in the IPYNB file. You can install Matplotlib using pip command: pip install matplotlib.

1. Seaborn - Seaborn is a Python library based on Matplotlib and used for data visualization. You need to have Seaborn installed on your system to use it in the IPYNB file. You can install Seaborn using pip command: pip install seaborn.

Once you have installed all the above software, you can run the IPYNB file in Jupyter Notebook. You may also need to have access to the CSV file being loaded with pd.read\_csv() if you're planning to run the code successfully.


**Project Screenshots** 

Heatmap Data Visualization
<img width="589" alt="Screen Shot 2023-03-07 at 11 41 17 AM" src="https://user-images.githubusercontent.com/115778006/223335857-5ce62781-e526-4869-a2c5-3058ffebf6bf.png">

Lineplots
<img width="1010" alt="Screen Shot 2023-03-06 at 11 14 25 PM" src="https://user-images.githubusercontent.com/115778006/223335409-dcbe3c33-9c26-484d-bf91-83a0f9bda667.png">

Subplots
<img width="1018" alt="Screen Shot 2023-03-06 at 11 15 14 PM" src="https://user-images.githubusercontent.com/115778006/223335346-e3975545-d025-4f23-95bf-de192a2d62d0.png">


Scatterplot

<img width="453" alt="Screen Shot 2023-03-07 at 11 42 19 AM" src="https://user-images.githubusercontent.com/115778006/223335809-8df6bf1c-2eb8-47cc-a33c-71b9fd493ac8.png">

**Contact Information**

Created by - Kaustubh Yadav
