# **RFM Analysis**
<img align=center src = "attachment:841fe85b-4cbd-417c-9c21-23c6415b9634.png" width="900" >
Content:
    
1. [What is RFM Analysis](#1) 
    
* [What inforamtion we can reveal after performing RFM Analysis?](#2)
    
2. [About the dataset ](#3)
    
* [Definiton of Variables ](#4)
* [Business goal ](#5)
   
3. [Coding Part](#6)
* [1. Loading the Dataset & Checking Variables](#6)
* [2. Answering some analytical questions about the data](#7)
* [3. Data preprocessing](#8)
* [4. Getting R, F and M metrics](#9)
* [5. Converting R, F and M metrices to R, F and M scores](#10)
* [6. Calculating RFM score](#11)
* [7. Segmenting customers using RFM score.](#12)
4. [Conclusion](#13)
<a id = "1"></a>
# **What is RFM Analysis?**
RFM analysis is a technique for categorizing customers based on their purchasing behavior. This segmentation method allows marketing teams to target customers with personalized marketing campaigns. Instead of analyzing the entire customer base as a whole, it's better to segment them into homogenous groups, understand the traits of each group, and engage them with relevant campaigns.

RFM stands for **R**ecency, **F**requency, and **M**onetary value. That means we have to use these metrics in order to perform this method. So what are these values?
* **Recency** : The freshness of customer activity. It's the time difference between the last purchase date of the customer and the date of analysis.
* **Frequency** : The frequency of the customer transaction, means a total number of transactions.
* **Monetary** : Sum of each purchase that has been made by each customer.  

 <a id = "2"></a>
#### **What inforamtion we can reveal after performing RFM Analysis?**
* Who are your best customers?
* Which customers have a chance to churn?
* Who has the potential to become valuable customers?
* Who are your loyal customers?
* Who are your new customers?
* Which customers is critical to retain?
* Which group of customers is most likely to respond to your current campaign?
* Which customers are lost? 

and more

#### **After a brief explanation of what is RFM let's move on to performing RFM to real-life data**


 <a id = "3"></a>
### **About the dataset :**
* This Online Retail II data set contains all the transactions occurring for a UK-based and registered, non-store online retail between 01/12/2009 and 09/12/2011.The company mainly sells unique all-occasion gift-ware. Many customers of the company are wholesalers.
 <a id = "4"></a>
### **Definiton of Variables :**
1. **Invoice:** Invoice number, unique identifier variable for each transaction. Refund invoice numbers starts with "C"
2. **StockCode:** Unique product code
3. **Description:** Product name
4. **Quantity:** The number of product in the invoice
5. **InvoiceDate:** Date and time of the purchase
6. **Price:** Unit price of a product (in terms of Sterlin)
7. **CustomerID:** Unique customer identifier
8. **Country:** Residential country of customers

 <a id = "5"></a>
### **Business goal**
* We want to segement the Customers based on RFM so that the company can target its customers efficiently.

 <a id = "6"></a>
# **Let's dive into coding part.**
### 1. Loading the Dataset & Checking Variables