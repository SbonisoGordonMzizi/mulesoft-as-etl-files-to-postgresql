# MuleSoft Data Integration Project
### Overview
This MuleSoft project demonstrates the integration of multiple data sources, including CSV and Excel files, and loads the extracted and processed data into a PostgreSQL database. It uses MuleSoft Anypoint Studio to build the ETL (Extract, Transform, Load) process, connecting to external data sources and performing data transformations before saving the data into the database.

### Features
- **Extract:** Reads data from CSV and Excel files.
- **Transform:** Processes and transforms the extracted data as per business requirements.
- **Load:** Inserts the transformed data into a PostgreSQL database.
- **Error Handling:** Built-in error handling for data format issues and database connection problems.
- **Logging:** Logs each stage of the ETL process for tracking and debugging.

### Prerequisites
To run this project, you will need the following installed:

- MuleSoft Anypoint Studio
- Java JDK 8 or higher
- PostgreSQL Database
- MuleSoft Database Connector
- MuleSoft File Connector

### How It Works
1. **Extract:** The MuleSoft flows read data from CSV and Excel files using the File Connector.
2. **Transform:** Data is transformed into a common structure, ensuring it can be processed correctly and mapped to the PostgreSQL schema.
3. **Load:** The processed data is loaded into a PostgreSQL database using the Database Connector.

### Flows Overview
1. **Main Flow:** Responsible for the orchestration of the ETL process, triggering the extract, transform, and load sub-flows.
2. **Error Handling Flow:** Catches and logs any errors that occur during the ETL process, ensuring robustness and traceability.
3. **Database Insert Flow:** Handles the insertion of transformed data into the PostgreSQL database.

