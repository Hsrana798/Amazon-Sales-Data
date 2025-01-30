
# Analyze and Provide Insights on Amazon Sales Report
 
📊 **A comprehensive Power BI dashboard for analyzing Amazon sales trends, product performance, fulfillment efficiency, customer segmentation, and geographical distribution.**  

### Power BI Dashboard Link: https://drive.google.com/drive/folders/1mkpGzpq-YW9W9j0GSmNlLPQD0Xv8E2-A?usp=sharing

---

## **📌 Project Overview**  
This project analyzes Amazon sales data to provide actionable insights into **sales performance, product trends, fulfillment methods, customer behavior, and regional distribution**. The dashboard helps businesses make **data-driven decisions to optimize inventory, fulfillment efficiency, and marketing strategies**.  

---

## **🎯 Key Objectives**  
✔️ **Sales Overview** – Track revenue trends, total orders, and order statuses.  
✔️ **Product Analysis** – Identify top-selling categories and sales distribution.  
✔️ **Fulfillment Analysis** – Compare Amazon-fulfilled vs. merchant-fulfilled orders.  
✔️ **Customer Segmentation** – Analyze buying behavior and customer distribution.  
✔️ **Geographical Analysis** – Visualize sales across different locations.  
✔️ **Business Insights** – Provide key recommendations for improving sales strategies.  

---

## **📂 Dataset Details**  
📄 **File Name:** `Amazon Sale Report.csv`  
📊 **Records:** Thousands of transaction-level sales data  
📝 **Fields:**  
- **Order Details:** Order ID, Date, Status, Fulfillment Method, Sales Channel  
- **Product Information:** Category, Size, Quantity, Amount  
- **Shipping Details:** Ship City, Ship State, Ship Country, Postal Code  
- **Customer Type:** Amazon & Non-Amazon  

---

## **🛠️ Power BI Implementation**  

### **1️⃣ Data Cleaning & Transformation (Power Query)**  
✅ Removed duplicate records based on `Order ID`.  
✅ Filled missing values (`Amount` set to `0` for canceled orders).  
✅ Converted `Date` column to the correct format for time intelligence.  

### **2️⃣ Data Modeling**  
- **Single-table model used for faster analysis.**  
- No additional relationships were required.  

### **3️⃣ DAX Measures & Calculations**  
Here are some key DAX measures used in the project:  

#### **🔹 Total Sales**
```DAX
Total Sales = SUM('Amazon Sale Report'[Amount])
```
#### **🔹 Total Orders**
```DAX
Total Orders = DISTINCTCOUNT('Amazon Sale Report'[Order ID])
```
#### **🔹 Average Order Value**
```DAX
Avg Order Value = DIVIDE(SUM('Amazon Sale Report'[Amount]), DISTINCTCOUNT('Amazon Sale Report'[Order ID]))
```
#### **🔹 Fulfillment Effectiveness**
```DAX
Fulfillment Effectiveness = 
DIVIDE(
    COUNTROWS(FILTER('Amazon Sale Report', 'Amazon Sale Report'[Status] = "Delivered")),
    COUNTROWS('Amazon Sale Report')
) * 100
```

---

## **📊 Dashboard Pages & Visualizations**  
This Power BI report is divided into **six pages**, each covering a different aspect of the business.

### **1️⃣ Sales Overview 📈**  
✔️ **KPIs:** Total Sales, Total Orders, AOV  
✔️ **Visuals:**  
- **Line Chart** – Sales trends over time  
- **Pie Chart** – Order status breakdown  
- **Bar Chart** – Sales by sales channel  

---

### **2️⃣ Product Analysis 🛍️**  
✔️ **KPIs:** Best-Selling Category, Monthly Sales  
✔️ **Visuals:**  
- **Bar Chart** – Top-selling product categories  
- **Matrix Heatmap** – Monthly sales by product category  
- **Pie Chart** – Product sales distribution  

---

### **3️⃣ Fulfillment Analysis 🚚**  
✔️ **KPIs:** Fulfillment Effectiveness, Amazon vs. Merchant Orders  
✔️ **Visuals:**  
- **Stacked Bar Chart** – Order fulfillment performance  
- **Pie Chart** – Fulfillment method breakdown  

---

### **4️⃣ Customer Segmentation 👥**  
✔️ **KPIs:** B2B Sales, Order Frequency  
✔️ **Visuals:**  
- **Bar Chart** – Customer segmentation by purchase frequency  
- **Pie Chart** – Customer breakdown  

---

### **5️⃣ Geographical Analysis 🌍**  
✔️ **KPIs:** Total Revenue by Region, State-wise Sales  
✔️ **Visuals:**  
- **Map Chart** – Sales distribution across locations  
- **Bar Chart** – Top-selling states and cities  

---

### **6️⃣ Business Insights 💡**  
✔️ **KPIs:** Sales Target vs. Actual Sales, Canceled Orders %  
✔️ **Visuals:**  
- **Gauge Chart** – Sales performance vs. target  
- **Heatmap (Matrix Table)** – High-performing products over time  
- **KPI Cards** – Key business takeaways  

---

## **📌 Key Insights & Recommendations**  

### **🛒 Sales Performance**  
✅ **Peak sales months** should be leveraged for seasonal marketing.  
✅ **Repeat customers drive revenue**, so customer retention programs should be introduced.  
✅ **High cancellation rates** impact revenue—improve customer communication and product descriptions.  

### **📦 Product & Inventory Management**  
✅ **Top-selling products should be prioritized** in promotions and stock management.  
✅ **Slow-moving items** should have discounts or bundling strategies.  

### **🚚 Fulfillment & Logistics**  
✅ **Amazon-fulfilled orders have better success rates**—more sellers should be encouraged to use FBA.  
✅ **Delayed shipping regions should be optimized** with better courier partnerships.  

### **📍 Customer & Regional Targeting**  
✅ **B2B customers generate more revenue**—target them with bulk discounts.  
✅ **Expand in high-sales regions** while boosting marketing in low-performing areas.  

---

## **🚀 Future Enhancements**  
📌 Integrate **customer feedback data** to analyze satisfaction and improve service.  
📌 Implement **predictive analytics** for sales forecasting and demand planning.  
📌 Add **competitor pricing analysis** for strategic product pricing.  

---

## **📥 Installation & Usage**  
### **🔹 How to Open the Power BI Report**
1. Download `Amazon Sales Report.pbix`.  
2. Open with **Power BI Desktop** (latest version recommended).  
3. Load dataset (`Amazon Sale Report.csv`) if required.  
4. Explore dashboards and interact with slicers & filters.  

---

## **🛠️ Tools & Technologies Used**  
✔️ **Power BI Desktop** – Data visualization and report building  
✔️ **Power Query** – Data cleaning and transformation  
✔️ **DAX (Data Analysis Expressions)** – Measures and calculations  
✔️ **Excel/CSV** – Data storage and management  
✔️ **Word** – Documentation  
---

## **🤝 Contributing**  
Contributions are welcome! Feel free to fork this repository, create issues, or suggest improvements.  

---

## **📩 Contact & Support**  
If you have any questions, feel free to reach out:  
📧 Email: **harshrana8460@gmail.com**  
💬 LinkedIn: **https://www.linkedin.com/in/harsh-data-analyst** 
---
### Contact No: +91 8460199614 (Harsh Rana)

Thank You So Much InnoByte Service
---
