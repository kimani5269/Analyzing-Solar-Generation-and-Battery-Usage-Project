# Analyzing-Solar-Generation-and-Battery-Usage-Project
The project analyzes solar electricity generation, electricity usage, and battery usage data to understand the potential benefits of using a battery system to store excess solar electricity. Through the project I utilized SQL and python programming language and various libraries including pandas for data manipulation, numpy for numerical operations, matplotlib for data visualizations, and datetime for handling time-related data. 
I did the following in the project:
   a. Performing data visualizations and checks.
   b. Calculating electricity bought. 
   Calculating excess solar generation.
   Modelling the battery charge level.

Project Steps:
1. Data Visualizations and checks.
The project begins by loading the provided data SQL Postgres into a pandas DataFrame. The data contains information about solar electricity generation, electricity usage, and other relevant parameters. The goal of this step is to visualize and compare the average solar electricity generation and electricity usage for each hour in a day.

2. Calculating electricity bought
In this step, the project calculates the electricity needed to be bought from the provider by subtracting the solar electricity generation from the electricity usage. The numpy library is used to efficiently perform element-wise subtraction and limit the result to non-negative values.

3. Calculating excess solar generation
The excess solar electricity generated is calculated by subtracting the electricity usage from the solar electricity generation. Similar to Step (ii), numpy is used to perform element-wise subtraction and limit the result to non-negative values.

4. Modelling battery charge level
This step models the cumulative battery charge level over time. The project assumes a maximum battery capacity of 12.5 kWh. The battery charge level is updated iteratively using a loop that considers the excess solar electricity generated and limits the charging to the battery's maximum capacity.

5. Calculating electricity bought with battery
The electricity bought when using the battery is calculated by subtracting the excess solar generation from the previously calculated electricity bought. This accounts for the electricity stored in the battery that can be used instead of buying from the provider.

6. Calculating savings from installing a battery
To quantify the potential savings from installing a battery, the project calculates the cost difference between buying electricity from the provider without a battery and buying electricity with a battery. The electricity price is assumed to be $0.17 per kWh.

Conclusion
This project demonstrates the process of analyzing solar electricity generation, electricity usage, and battery usage data. It showcases various data manipulation techniques, calculations, and data visualization methods using Python and its libraries. The results provide insights into the potential benefits of utilizing a battery system to store excess solar electricity, leading to potential cost savings and increased energy efficiency.
