# Capstone-Project-Summer-Analytics-2025
Capstone Project for the Summer Analytics 2025 of Consulting &amp; Analytics Club

 Dynamic Pricing for Urban Parking Lots
Real-time, data-driven pricing engine for urban parking lots based on demand, traffic, and vehicle factors. Built for the Summer Analytics 2025 capstone project hosted by the Consulting & Analytics Club × Pathway.
________________________________________
📌 Project Overview
Static parking prices lead to inefficiencies like overcrowding or underutilization. This project implements dynamic pricing models for 14 parking lots using real-time data such as:
•	Occupancy levels
•	Queue length
•	Vehicle type
•	Nearby traffic conditions
•	Special days/events
The goal is to maximize utilization and optimize revenue by adjusting prices in real-time.
________________________________________
🛠 Tech Stack
Technology	Purpose
Python	Core development
Pandas	Data manipulation & processing
NumPy	Numerical operations
Bokeh	Interactive visualizations
Google Colab	Development & execution environment
Pathway	Real-time stream simulation 
________________________________________
🧠 Models Implemented
1.	Baseline Linear Model – Price increases proportionally to occupancy
2.	Demand-Based Model – Considers queue, traffic, vehicle weight, special days
3.	(Optional) Competitive Model – Uses location to adjust price based on nearby lots
________________________________________
🧱 Architecture Diagram (Mermaid)
    A[Raw CSV Dataset] --> B[Data Cleaning + Feature Mapping]
    B --> C1[Baseline Pricing Model]
    B --> C2[Demand-Based Model]
    C1 --> D[Combine Predictions]
    C2 --> D
    D --> E[Bokeh Visualizer]
________________________________________
🔄 Workflow Explained
1.	Data Ingestion:
o	Load dataset with 73 days of 30-min interval data
o	Combine date & time to single timestamp
2.	Feature Engineering:
o	Map categorical features to numeric (traffic, vehicle type)
o	Sort and group by parking lot
3.	Model Application:
o	Model 1: Iteratively compute price based on occupancy
o	Model 2: Calculate demand function using weighted feature contributions
4.	Visualization:
o	Use Bokeh to create interactive time-series plots for each parking lot
o	Compare pricing strategies across time
5.	(Optional) Model 3:
o	Compute distances between lots
o	Adjust price based on competitor load and cost (future scope) 
________________________________________
📌 Submission Checklist
•	All models implemented
•	Markdown report written
•	Visualizations integrated
•	Colab-executable notebook
•	Model 3 rerouting logic (optional)
________________________________________
✨ Future Improvements
•	Add Pathway streaming simulation
•	Real-time competitor price adjustment
•	API integration with live parking systems

