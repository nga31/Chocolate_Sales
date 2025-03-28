# Analysis Chocolate Sale
## Presented by Kim Nga
# 1. Goals of the project
### Mục đích : Phân tích doanh số bán hàng và tìm kiếm nguồn khách hàng tiềm năng trên thị trường.
### Outcome : Tăng doanh thu, mở rộng thị trường
# 2. Data sources used
### Datasets: Chocolate_sales.Csv
### Sources: https://www.kaggle.com/datasets/atharvasoundankar/chocolate-sales?select=Chocolate+Sales.xlsx
# 3. Data overview
## 3.1 What is the Data?
### Dữ liệu bán hàng của các sản phẩm Chocolate tại thị trường Australia, Canada, India, New Zealand, UK, USA. 
### Thời gian phân tích : 01/2022 - 08/2022
## 3.2 Description "Columns"
  ### Date : thời gian thực tế bán hàng
  ### Product Name : Tên sản phẩm của từng loại Chocolate bán ra
  ### Boxed Shipped : Ghi nhận số kiện hàng đã được vận chuyển.
  ### Sales person : Chuyên viên bán hàng tại công ty.
  ### Sales : Ghi nhận doanh số bán ra tại mỗi thời điểm.
  ### Country : Các thị trường được bán ra.
# 4. Tools and technologies applied
## 4.1. Python on Google Colab
### 4.1.1 Import data & Load the data
  "import pandas as pd
      import matplotlib.pyplot as plt
      import seaborn as sns
      import statsmodels.api as sm"
    
  df = pd.read_csv("/content/drive/MyDrive/Chocolate Sales.csv")"
 ### 4.1.2 Data Cleaning
#### Display the first few rows of the data
##### df.head()

<img width="709" alt="Ảnh chụp Màn hình 2025-03-24 lúc 22 33 33" src="https://github.com/user-attachments/assets/87dfe40f-5395-46aa-8caf-aae79b65c6a7" />

#### Display basic information

##### df.info()

###### <img width="398" alt="image" src="https://github.com/user-attachments/assets/fca2d888-6d8f-4929-96d3-bfb1d6227988" />

##### df.describe()

###### <img width="247" alt="image" src="https://github.com/user-attachments/assets/b7a4a624-de12-483c-8d0c-51e208efcd22" />

##### Duplicate Rows "df.duplicated().sum()" & missing values " df.isnull().sum()"

###### <img width="426" alt="image" src="https://github.com/user-attachments/assets/03ddb4a3-ae2b-4cd2-bf1b-c200c0d28b48" />

## 4.2. Power BI
### Data Visualizations
#### Sales Highlights

#### Sales Trends

# 5. Key insights discovered
### Sale by Country

  " plt.figure(figsize=(10, 6))
    sns.countplot(x='Country', data=df, palette='viridis')
    plt.title('Sales Count by Country', fontsize=14)
    plt.xlabel('Country', fontsize=12)
    plt.ylabel('Sales Count', fontsize=12)
    plt.xticks(rotation=45, ha='center')
    plt.tight_layout()
    plt.show() "
    
![image](https://github.com/user-attachments/assets/a098d611-6b7e-431a-8ed0-20bc9d2a9e5d)

# 6. Recommendations based on analysis results

 ### Với dữ liệu phân tích, đề xuất phương án: 
##### - Đề xuất đội sales tìm hiểu khách hàng ở New Zealand để đẩy mạnh tang doanh số 
##### - Làm việc với team MKT để chạy quảng cáo vào tháng 02 và tháng 04/2023
##### - Phân tích và dự toán ngân sách cho dự án phát triển mở thị trường Châu Á.

# 7. Action plan

## <img width="832" alt="image" src="https://github.com/user-attachments/assets/d42ce4bd-82a3-498b-82ad-cdfb5a2a4747" />
