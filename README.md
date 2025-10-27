# EXNO-6-DS-DATA VISUALIZATION USING SEABORN LIBRARY

# Aim:
  To Perform Data Visualization using seaborn python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:
```
 import pandas as pd
 import seaborn as sns
 import matplotlib.pyplot as plt
 df=pd.read_csv("/content/titanic_dataset (1).csv")
 df.head()
```

<img width="1274" height="228" alt="image" src="https://github.com/user-attachments/assets/e8de7c58-62d2-4fbb-b667-78e0ad08adce" />

```
x=[1,2,3,4,5]
y=[3,6,2,7,1]
sns.lineplot(x=x,y=y)
plt.title('Line Plot')
```

<img width="639" height="508" alt="image" src="https://github.com/user-attachments/assets/7948ec96-20ea-4385-b95d-e549959f101a" />

```
x=[1,2,3,4,5]
y1=[3,5,2,6,1]
y2=[1,6,4,3,8]
y3=[5,2,7,1,4]
sns.lineplot(x=x,y=y1)
sns.lineplot(x=x,y=y2)
sns.lineplot(x=x,y=y3)
plt.title('Multi Line Plot')
```

<img width="605" height="519" alt="image" src="https://github.com/user-attachments/assets/13402002-f1ec-44d4-90c8-e8a58e6cedf7" />

```
 plt.figure(figsize=(8,5))
 sns.barplot(x='Embarked',y='Fare',data=df,palette='rainbow')
 plt.title("Fare Of Passenger By Embarked Town")
```

<img width="773" height="524" alt="image" src="https://github.com/user-attachments/assets/5684f24c-0888-4628-adb5-e4c8ea875a80" />

```
 sns.scatterplot(x="Age", y="Fare", data=df)
 plt.title('Scatterplot of Age vs Fare')
 plt.show()
```

<img width="652" height="511" alt="Screenshot 2025-10-27 114205" src="https://github.com/user-attachments/assets/cad4fe27-1f97-4ab1-a821-edafd24523eb" />

```
sns.scatterplot(x="Age", y="Fare", size="Pclass", data=df, sizes=(30, 200))
plt.title('Bubble Chart of Age vs Fare, Size by Passenger Class')
plt.show()
```

<img width="670" height="506" alt="image" src="https://github.com/user-attachments/assets/05eaa873-2afc-47b0-adc4-861dab324b31" />

```
 sns.histplot(data=df,x="Pclass",hue="Survived",kde=True)
```

<img width="643" height="501" alt="image" src="https://github.com/user-attachments/assets/5e898e46-b954-40c7-83dd-af9badcc357c" />

```
sns.boxplot(x='Pclass',y='Age',data=df,palette='rainbow')
plt.title("Age By Passenger Class")
```

<img width="637" height="499" alt="Screenshot 2025-10-27 114449" src="https://github.com/user-attachments/assets/420d4e7d-3efa-47d2-98ca-4c217c01c842" />

```
 sns.violinplot(x="Pclass", y="Fare", data=df)
 plt.title('Violin Plot of Fare by Passenger Class')
 plt.show()
```

<img width="675" height="508" alt="image" src="https://github.com/user-attachments/assets/82153d5e-0a92-46c5-85ee-317ff842ed0d" />

```
 sns.kdeplot(data=df['Age'], shade=True)
 plt.title('Density Plot of Passenger Ages')
 plt.show()
```

<img width="668" height="504" alt="Screenshot 2025-10-27 114615" src="https://github.com/user-attachments/assets/805c6430-9ad4-4db2-92f5-e8363a0883cd" />

```
 numeric_df = df.select_dtypes(include=['float64', 'int64'])
 corr_matrix = numeric_df.corr()
 sns.heatmap(corr_matrix, annot=True, cmap='coolwarm')
 plt.title('Heatmap of Titanic Dataset')
 plt.show()
```

<img width="676" height="562" alt="Screenshot 2025-10-27 114742" src="https://github.com/user-attachments/assets/88f29847-8cda-4929-8bb0-94cebe09e358" />


# Result:
Thus , to perform data visualization using seaborn python library for the given datas is successfully completed.

