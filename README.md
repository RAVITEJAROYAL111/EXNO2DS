# EXNO2DS
# AIM:
      To perform Exploratory Data Analysis on the given data set.
      
# EXPLANATION:
  The primary aim with exploratory analysis is to examine the data for distribution, outliers and anomalies to direct specific testing of your hypothesis.
  
# ALGORITHM:
STEP 1: Import the required packages to perform Data Cleansing,Removing Outliers and Exploratory Data Analysis.

STEP 2: Replace the null value using any one of the method from mode,median and mean based on the dataset available.

STEP 3: Use boxplot method to analyze the outliers of the given dataset.

STEP 4: Remove the outliers using Inter Quantile Range method.

STEP 5: Use Countplot method to analyze in a graphical method for categorical data.

STEP 6: Use displot method to represent the univariate distribution of data.

STEP 7: Use cross tabulation method to quantitatively analyze the relationship between multiple variables.

STEP 8: Use heatmap method of representation to show relationships between two variables, one plotted on each axis.

## CODING AND OUTPUT
           <<INCLUDE YOUR CODING AND OUTPUT SCREENSHOTS>>
     import pandas as pd
     import numpy as np
    import seaborn as sns
    data=pd.read_csv("titanic_dataset.csv")
    data
<img width="1042" height="448" alt="image" src="https://github.com/user-attachments/assets/ffad59d7-355a-495a-8ef1-c8cc62bf2d97" />

    data.info()
<img width="680" height="592" alt="image" src="https://github.com/user-attachments/assets/937c3abe-4478-4cf6-881c-cfce156f62dc" />

    data.describe()
<img width="1041" height="432" alt="image" src="https://github.com/user-attachments/assets/c52a5d72-1a3b-4100-b4e9-3f3ce1439817" />

    data.dtypes
<img width="446" height="460" alt="image" src="https://github.com/user-attachments/assets/e2084e16-5382-48a9-8432-9e2f37b9873d" />

    data.shape
  <img width="280" height="123" alt="image" src="https://github.com/user-attachments/assets/92125a84-3fca-466d-847f-6f81b3d7641a" />

    data.value_counts()
<img width="1030" height="508" alt="image" src="https://github.com/user-attachments/assets/aec38ecd-46fe-4046-b1e9-1b1e516c1c87" />

      sns.countplot(data=data,x='Survived')
<img width="1036" height="756" alt="image" src="https://github.com/user-attachments/assets/41e48b3c-bb69-4872-adf2-92f39e498aff" />

    corr=data.corr(numeric_only=True)
    sns.heatmap(corr,annot=True)
<img width="1037" height="847" alt="image" src="https://github.com/user-attachments/assets/fa1c45fb-41ac-4288-8fd9-5bb518a565c0" />

# RESULT
Exploratory Data Analysis (EDA) was successfully performed on the given dataset using Python libraries. The data was analyzed using summary statistics and visualizations to identify patterns, relationships, missing values, and outliers in the dataset.
 <<INCLUDE YOUR RESULT HERE>>
