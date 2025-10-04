# 📊 E-Commerce Sales Performance Dashboard

## 🎯 Project Overview

Interactive sales analytics dashboard built using **Microsoft Power BI** to analyze e-commerce performance across multiple dimensions including regions, product categories, customer segments, and temporal trends. This dashboard provides actionable insights for data-driven business decision-making.

**Built as part of:** Data Analyst Internship - Task 8

---

## 📈 Key Metrics at a Glance

|         Metric       |      Value |
|----------------------|------------|
| 💰 **Total Sales**  |    $12.64M |
| 📈 **Total Profit** |     $1.47M |
| 📦 **Total Orders** |     25,040 |
| 📊 **Profit Margin** |     11.6% |
| 🌍 **Regions Covered** | 12+ Global Markets |
| 📦 **Product Categories** | 3 (Technology, Furniture, Office Supplies) |

---

## 🛠️ Tools & Technologies

- **Power BI Desktop** - Data visualization and dashboard development
- **Power Query** - Data transformation and cleaning
- **Dataset:** E-commerce transactional data with 25,000+ orders

---

## 📁 Dataset Information

### Data Structure

**Order Information:**
- Row_ID, Order_ID, Order_Date, Ship_Date, Ship_Mode, Order_Priority

**Customer Details:**
- Customer_ID, Customer_Name, Segment (Consumer/Corporate/Home Office)

**Geographic Dimensions:**
- City, State, Country, Market, Region, Postal_Code

**Product Hierarchy:**
- Product_ID, Product_Name, Category, Sub_Category

**Financial Metrics:**
- Sales, Profit, Quantity, Discount, Shipping_Cost

### Data Scope
- **Time Period:** 12 months (January - December)
- **Total Records:** 25,040 orders
- **Geographic Coverage:** Global (12+ regions)
- **Product Lines:** 3 major categories with multiple sub-categories

---

## 📊 Dashboard Components

### 🎯 Interactive Filters (Slicers)
1. **Region Slicer** - Filter by geographic region (Africa, Canada, Caribbean, Central, etc.)
2. **Category Slicer** - Filter by product category (Furniture, Office Supplies, Technology)

### 💳 Key Performance Indicators (KPI Cards)
- **Total Sales:** $12.64M - Aggregate revenue across all transactions
- **Total Profit:** $1.47M - Net profit after costs and discounts
- **Total Orders:** 25.04K - Unique order count

### 📈 Main Visualizations

#### 1. 📉 Monthly Sales Trend (Line Chart)
- **Purpose:** Track sales performance over time
- **Insight:** Identifies seasonal patterns and growth trends
- **Key Finding:** November peak at $1.53M, February low at $0.54M
- **Color:** Green background for easy trend identification

#### 2. 📊 Sales Performance by Region (Bar Chart)
- **Purpose:** Compare regional sales performance
- **Insight:** Highlights top-performing and underperforming markets
- **Key Finding:** Central region leads with $2.82M (22% of total)
- **Color:** Orange background with blue bars for contrast
- **Feature:** Sorted descending by sales value

#### 3. 🍩 Sales Distribution by Category (Donut Chart)
- **Purpose:** Show product mix composition
- **Insight:** Reveals category dominance and revenue diversification
- **Key Finding:** Technology 37.53%, Furniture 32.52%, Office Supplies 29.96%
- **Color:** Purple background with distinct segment colors
- **Feature:** Percentage labels for clear understanding

---

## 🔍 Key Insights & Findings

### 1️⃣ Regional Performance Analysis

**Finding:**
- **Central region** generates highest sales at **$2.82M** (22% of total revenue)
- **Top 3 regions:** Central > South ($1.61M) > North ($1.25M)
- **Lowest performer:** West region at $0.73M (5.8% of total)
- **Performance gap:** 3.9x difference between best and worst regions

**Business Impact:**
- Significant growth opportunity in underperforming regions
- Central region's strategies should be studied and replicated
- Resource reallocation needed for regional optimization

---

### 2️⃣ Temporal Sales Trends

**Finding:**
- **Peak month:** November at $1.53M
- **Clear seasonality:** Q4 (Oct-Dec) accounts for 32% of annual sales
- **Lowest month:** February at $0.54M (65% below peak)
- **Holiday boost:** 83% sales increase from September to November

**Business Impact:**
- Inventory planning must account for 2.8x demand surge in Q4
- Marketing investment should increase before October
- Promotional campaigns needed during Jan-Feb to stabilize revenue
- Staffing augmentation required during peak season

---

### 3️⃣ Product Category Analysis

**Finding:**
- **Technology leads:** 37.53% market share (~$4.74M)
- **Balanced portfolio:** All three categories contribute 30%+ each
- **Category distribution:**
  - Technology: 37.53%
  - Furniture: 32.52%
  - Office Supplies: 29.96%

**Business Impact:**
- Diversified revenue stream reduces business risk
- No over-reliance on single category
- Cross-selling opportunities between complementary products
- All categories warrant strategic investment

---

### 4️⃣ Profitability & Efficiency

**Finding:**
- **Profit margin:** 11.6% ($1.47M profit on $12.64M sales)
- **Average order value:** $505 per order
- **Order volume:** 25,040 orders demonstrating strong customer base

**Business Impact:**
- Moderate profit margin indicates optimization opportunities
- High AOV suggests B2B or premium B2C model
- Focus on margin improvement through cost optimization

---

## 💡 Strategic Recommendations

### 1. Regional Expansion
- Increase marketing investment by 50% in West, Central Asia, and Africa
- Implement "Central region playbook" in underperforming markets
- Consider regional partnerships for local market penetration

### 2. Seasonal Optimization
- Build inventory 2-3 months before Q4 (July-August procurement)
- Launch early holiday promotions in September
- Implement dynamic pricing during off-peak months (Jan-Feb)

### 3. Category Management
- Maintain balanced investment across all three categories
- Create cross-category product bundles (e.g., Home Office Package)
- Analyze sub-category profitability for optimization

### 4. Profitability Enhancement
- Target 15% profit margin (current: 11.6%)
- Negotiate better shipping rates (10-15% cost reduction)
- Optimize product mix toward higher-margin items
- Implement customer loyalty program


## 📚 Technical Implementation

### Data Transformations (Power Query)
- Converted Order_Date to proper datetime format
- Created Month-Year column: `Date.ToText([Order_Date], "MMM-yyyy")`
- Created Month-Num for chronological sorting: `Date.Month([Order_Date])`
- Handled missing values and removed duplicates
- Verified data types for all columns

### Visualization Specifications
- **Line Chart:** Continuous time-series, 3px line width, data labels enabled
- **Bar Chart:** Horizontal bars sorted descending, value labels displayed
- **Donut Chart:** Inner radius 50%, percentage labels, legend on right
- **KPI Cards:** Large callout values (28pt), contextual background colors

### Color Palette
- **Green (#00FF00)** - Positive trends, growth indicators
- **Orange (#FF6600)** - Comparative analysis, regional focus
- **Purple (#CC99FF)** - Category distribution, diversity
- **Blue (#0078D4)** - Data bars, primary accent
- **White/Gray (#F5F5F5)** - Background, neutral space

---

## 💼 Business Impact

### Strategic Value
- **Time Savings:** Reduces analysis time from hours to minutes
- **Decision Support:** Enables real-time, data-driven decisions
- **Transparency:** Shared dashboard improves cross-functional alignment
- **Scalability:** Framework easily extends to additional metrics

### Use Cases
1. **Executive Leadership:** High-level performance monitoring
2. **Sales Teams:** Regional and category performance tracking
3. **Marketing:** Campaign effectiveness and seasonal planning
4. **Operations:** Inventory planning and demand forecasting
5. **Finance:** Revenue forecasting and profitability analysis

---

## 🎓 Learning Outcomes

Through this project, I developed expertise in:

✅ **Data Analysis**
- Extracting meaningful insights from large datasets
- Identifying trends, patterns, and anomalies
- Statistical reasoning and business intelligence

✅ **Data Visualization**
- Selecting appropriate chart types for different data stories
- Creating clear, intuitive visual representations
- Applying color theory and design principles

✅ **Power BI Skills**
- Data import and ETL processes
- Power Query transformations
- Interactive dashboard development
- Visual formatting and optimization

##  Acknowledgments

- Dataset: E-commerce sales data
- Tools: Microsoft Power BI Desktop
- Inspiration: Modern business intelligence best practices





---

**⭐ If you found this project helpful, please star this repository!**

---

*This dashboard demonstrates proficiency in data visualization, business intelligence, and analytical thinking—core competencies for data analyst roles.*
