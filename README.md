# workshop-Multivariate-analysis
#Code
import pandas as pd
import seaborn as sns
excel_file='/content/FlightInformation.xlsx'
df=pd.read_excel(excel_file)
print(df)
![Screenshot (68)](https://user-images.githubusercontent.com/96919035/229974860-62f2b40f-cdba-4a77-afdd-aa865fc3374c.png)
![Screenshot (69)](https://user-images.githubusercontent.com/96919035/229975999-a9d8440c-3862-4051-9c67-2b98a36f5531.png)
df.dtypes
![Screenshot (70)](https://user-images.githubusercontent.com/96919035/229974978-e3158a37-f897-48eb-a255-938d675b6531.png)
sns.scatterplot(y=df['Price'],x=df['Total_Stops'],data=df)
![Screenshot (71)](https://user-images.githubusercontent.com/96919035/229976204-efc07d06-3ebe-4f89-81c1-b2a248cc48b9.png)
sns.barplot(y=df['Price'],x=df['Source'],data=df)
![Screenshot (72)](https://user-images.githubusercontent.com/96919035/229976247-c3f7e2ec-b041-493e-bc88-23eb194178a7.png)
df.info()
![Screenshot (73)](https://user-images.githubusercontent.com/96919035/229976281-41d2846a-0c16-4379-833c-c68dfa6efe21.png)
df.corr()
sns.heatmap(df.corr(),annot=True)
![Screenshot (74)](https://user-images.githubusercontent.com/96919035/229975639-dbe53f52-5ca7-4df5-841e-da5a107930ee.png)
