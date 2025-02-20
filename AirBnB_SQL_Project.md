# **AirBnB SQL Project**  

The CSV files used in this project can be found at the following link: [Google Drive](https://drive.google.com/drive/folders/1NGDWNP8carmOqTSM0lED237JxcJUPNwi?usp=drive_link).


## **📌 Project Description**  
This project focuses on analyzing **AirBnB listings in London, UK**. After performing exploratory data analysis on the listings, the goal was to identify **potential leads** for a hypothetical new **cleaning and maintenance service**.  

## **🛠️ Tech Stack**  
- **Database**: SQLite3  
- **Language**: SQL  

---

## **📊 Features**  
✅ Relational database creation  
✅ Table creation and data import  
✅ Exploratory data analysis using SQL  
✅ Basic report generation for insights  

---

## **📥 Installation & Setup**  

1. **Download Data**  
   - Get the relevant CSV files from [this Google Drive link](https://drive.google.com/drive/folders/1NGDWNP8carmOqTSM0lED237JxcJUPNwi?usp=drive_link).  

2. **Set Up SQLite3**  
   - If SQLite3 is not installed, download it from [SQLite Official Website](https://www.sqlite.org/download.html).  
   - Verify installation:  
     ```sh
     sqlite3 --version
     ```

3. **Create the Database**  
   - Open SQLite3 and create a new database:  
     ```sh
     sqlite3 airbnb_london.db
     ```

4. **Import the CSV Data into SQLite**  
   - Open SQLite shell and run:  
     ```sql
     .mode csv
     .import 'listings.csv' listings
     ```

5. **Run SQL Queries**  
   - Open SQLite and explore the data:  
     ```sh
     sqlite3 airbnb_london.db
     ```
   - Example query:  
     ```sql
     SELECT host_id, host_name, AVG(review_scores_cleanliness) AS avg_cleanliness 
     FROM listings 
     GROUP BY host_id 
     ORDER BY avg_cleanliness DESC;
     ```

---

## **🔎 Guiding Questions**  
This project explores **key questions** to extract meaningful insights from the dataset:  

1️⃣ **What are the 10 most reviewed listings?**  
2️⃣ **What are the top 5 most expensive neighbourhoods?**  
3️⃣ **Are any hosts fully booked for March 2025, and which hosts have the least number of available dates in March 2025?**  
4️⃣ **Who are the hosts with the least listings?**  
5️⃣ **Identify some hosts which may benefit from a new cleaning service provider.**  

---

## **🚀 Usage**  
This project serves as a **template** for:  
- Importing web-scraped data into a **relational database**  
- Performing **exploratory analysis** on structured data  
- Extracting **actionable insights** from raw datasets  

---

## **💡 Inspiration**  
The inspiration for this project was a **curiosity-driven deep dive** into AirBnB listing data. The goal was to **identify market opportunities** by finding hosts who might benefit from a **cleaning and maintenance service**.  

---

## **📌 Notes**  
- No contribution guidelines at the moment.  
- No specific license.  
