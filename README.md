# Internal Audit Process Automation

## Overview

The Internal Audit Process Automation project aims to streamline and enhance the efficiency of internal audit processes by automating data extraction, validation, and anomaly detection. This system leverages Python for data validation and anomaly detection, SQL for data extraction, and UiPath for robotic process automation. The automation significantly reduces manual effort, improves audit accuracy, and accelerates the audit cycle.

## Technologies Used

- **Python**
  - Pandas
  - NumPy
  - Scikit-learn
  - pyodbc
- **SQL**
- **Robotic Process Automation (UiPath)**

## Features

- Automated data extraction from the SQL database.
- Data validation checks to ensure data integrity.
- Anomaly detection using the Isolation Forest algorithm.
- Integration with UiPath for process automation, including data extraction, running Python scripts, and sending audit reports.

## Setup Instructions

### Prerequisites

1. **Python 3.x** installed on your system.
2. **Visual Studio Code (VS Code)** installed on your system.
3. **SQL Server** (or any other compatible SQL database) installed and running.
4. **UiPath Studio** installed on your system.
5. Basic knowledge of Python, SQL, and UiPath.

### Step-by-Step Setup

#### 1. Clone the Repository

```bash
git clone https://princemsd007/Internal-Audit-Process-Automation..git
cd internal-audit-process-automation
```
2. Set Up Python Evviornment
      1. Create and active  virtual enviornment
  ```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```
2. Install the required Python packages
3. Configure SQL Database
Ensure your SQL server is running and accessible. Update the connection details in the Python script (audit_process.py).

4. UiPath Setup
   1. Create a new process in UiPath Studio.
   2. Integrate the Python script using Python activities.
   3. Automate the workflow for data extraction, running Python scripts, and sending reports.
  
### UiPath Workflow

Create a new process in UiPath Studio.

Automate data extraction:
  . Use the Database activities to connect to the SQL database and extract audit data.
  
Run Python script:
  . Use the Python activities to invoke the Python script (audit_process.py)  
  
Process anomalies:
  . se the Excel activities to export anomalies detected by the Python script to an Excel file.
  . Use the Send Outlook Mail Message activity to email the audit report to relevant   stakeholders.


### Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or new features.

### License
This project is licensed under the MIT License - see the LICENSE file for details.






