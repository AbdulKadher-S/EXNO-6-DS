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

import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt

data = pd.read_csv('titanic_dataset.csv')

print(data.info())
print(data.head())

plt.figure(figsize=(6,4))
sns.countplot(x='Survived', data=data)
plt.title('Count of Survivors')
plt.show()

plt.figure(figsize=(6,4))
sns.countplot(x='Pclass', data=data)
plt.title('Passenger Count by Class')
plt.show()

plt.figure(figsize=(6,4))
sns.barplot(x='Sex', y='Survived', data=data)
plt.title('Survival Rate by Sex')
plt.show()

plt.figure(figsize=(8,5))
sns.histplot(data['Age'].dropna(), kde=True, bins=30)
plt.title('Age Distribution')
plt.show()

plt.figure(figsize=(6,4))
sns.countplot(x='Embarked', hue='Survived', data=data)
plt.title('Survival Count by Embarked Port')
plt.show()

plt.figure(figsize=(8,5))
sns.boxplot(x='Survived', y='Age', data=data)
plt.title('Age Distribution by Survival')
plt.show()

plt.figure(figsize=(8,6))
sns.heatmap(data.corr(), annot=True, cmap='coolwarm')
plt.title('Correlation Heatmap')
plt.show()

<img width="552" height="677" alt="Screenshot 2025-10-15 143005" src="https://github.com/user-attachments/assets/8085ea34-0457-4fe7-a9f3-d66fc90e99e8" />
<img width="922" height="748" alt="Screenshot 2025-10-15 143016" src="https://github.com/user-attachments/assets/83809e7b-c40e-46cc-b52e-294bd7299802" />
<img width="741" height="493" alt="Screenshot 2025-10-15 143023" src="https://github.com/user-attachments/assets/076c3f7e-9fce-4c79-b443-7ecb69a942c3" />
<img width="741" height="490" alt="Screenshot 2025-10-15 143029" src="https://github.com/user-attachments/assets/31c6dfc9-0e0f-41c6-918f-d1379bf172de" />
<img width="738" height="485" alt="Screenshot 2025-10-15 143035" src="https://github.com/user-attachments/assets/a4299457-1f29-4c78-ac96-8ac43df97c99" />
<img width="988" height="606" alt="Screenshot 2025-10-15 143041" src="https://github.com/user-attachments/assets/697d12e0-7cac-4ed1-92c7-e8aa250444da" />
<img width="740" height="482" alt="Screenshot 2025-10-15 143048" src="https://github.com/user-attachments/assets/2ff78003-8470-45df-8ec0-bb6f2081b9a8" />
<img width="984" height="583" alt="Screenshot 2025-10-15 143055" src="https://github.com/user-attachments/assets/dc5ec444-8784-4b68-ae07-45110a60aefc" />
<img width="743" height="483" alt="Screenshot 2025-10-15 143135" src="https://github.com/user-attachments/assets/6a3ec39b-33b8-40a8-bd74-49b116e16678" />
<img width="981" height="607" alt="Screenshot 2025-10-15 143143" src="https://github.com/user-attachments/assets/f0534957-9659-459c-b05e-f316b76debb2" />
<img width="986" height="740" alt="Screenshot 2025-10-15 143154" src="https://github.com/user-attachments/assets/e780e1b8-6494-4857-b83d-a11aa4c4e79b" />


# Result:
  The program was executed successfully.
