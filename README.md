# MIS 311-Individual Assignment: Shoe Price
# 1. Data overview
- **Source**: The dataset appears to be a compilation of shoe inventory or sales data, likely sourced from a retail or e-commerce platform, as it includes details on shoe brands, colors, sizes, and prices.
- **Number of rows & column**: The dataset contains 203 rows (including the header) and 4 columns: brand, color, size, and price.
- **Context/Background**: The dataset represents a collection of shoes with attributes such as brand (e.g., Crocs, Tresmode, Adidas), color (e.g., Black, Brown, Blue), size (ranging from 2 to 13), and price (ranging from 80 to 350). It likely serves purposes such as inventory management, pricing analysis, or market research for a shoe retailer or distributor. The variety of brands and colors suggests a diverse product catalog aimed at different customer preferences.
# 2. Data cleaning
- **Identify any duplicate rows and remove duplicate rows if necessary**
![Screenshot 2025-05-14 092052](https://github.com/user-attachments/assets/229ddedb-bfa3-46f4-8d6b-d1bbbc77e046)
   - The data indicates that **3 duplicate values** were found and removed from the dataset, leaving **199 unique values**. This means the data has been cleaned to some extent, improving accuracy for analysis.

![image](https://github.com/user-attachments/assets/be40d4cf-ff0f-4d30-9385-f0f5298c18e2)
- **Identify missing values and decide how to handle these missing values**
  - In the data, brand **Tory Bruch** is missing color and brand **Liberty** is also missing price.

![image](https://github.com/user-attachments/assets/0092bfae-8355-4179-b59a-3fa2fdec39b1)
-  I used impute values to replace the missing values with average or most frequent value
    - For the **Tory Burch** brand, the color was missing, so I filled it with "Black" as it is the most frequent color in the dataset, appearing approximately 49 times.
    - For the **Liberty** brand, the price was missing, so I calculate the average price based on the data to fill it (156+347+291)/3=265.
    - I chose to impute the missing value because it allows me to retain all the data without discarding any rows, which helps preserve the overall dataset size and integrity. Instead of losing potentially valuable information, imputation provides a reasonable estimate based on existing patterns such as using the most frequent color or the average price.

# 3. Descriptive Statistics 
![image](https://github.com/user-attachments/assets/8022d13f-43ca-4549-93a8-3bd648ac566d)
- The descriptive statistics in the image above reveal several important insights, but I will focus on just two key observations.
    - The average price is approximately **$211.81**, with a median of **$208.5**, indicating that the data is fairly symmetrically distributed. The mode is **$100**, which is significantly lower than the mean and median, suggesting that while most prices are centered around **$210**, a large number of products are priced at the lower end.
    - The standard deviation is about **$79.09**, indicating a wide spread of prices around the mean. The range of **$270** (from **$80 to $350**) meaning that prices vary greatly across the dataset. This may reflect different product categories or brand values.

![image](https://github.com/user-attachments/assets/36100d00-3661-41c8-bee4-2e2966822376)
- PUMA stands out with the highest average price at **$307**, well above the overall average of **$271.4**, suggesting it positions itself as a premium brand. In contrast, brands like Umbro, Reebok, and Liberty have lower average prices, indicating a more competitive and affordability-focused pricing strategy aimed at price-sensitive customers.

![image](https://github.com/user-attachments/assets/7d3d33ef-52be-4182-ad9c-f8ac2d5fd14e)
- The most preferred shoe color is **Black**, with **49 counts**, followed by **Brown** with **37 counts**, making them the dominant choices among consumers. This indicates a strong preference for classic, versatile colors, which may influence sales revenue and marketing strategies to prioritize these color for higher sales potential.
