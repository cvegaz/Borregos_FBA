# Borregos_FBA Project

## Overview
The Borregos_FBA project is designed to manage data for a collegiate American football team. It includes a MySQL database to store player information, physical test results, and biometric measurements.

## Project Structure
```
Borregos_FBA
├── data
│   ├── players.csv
│   ├── physical_tests.csv
│   └── biometrics.csv
├── scripts
│   ├── insert_data.py
│   └── update_data.py
├── sql
│   ├── create_tables.sql
│   └── insert_initial_data.sql
├── README.md
└── requirements.txt
```

## File Descriptions

- **data/players.csv**: Contains player data including first name, middle name, last name (paternal), last name (maternal), date of birth, position, academic program, and date of entry to the team.

- **data/physical_tests.csv**: Stores data related to physical tests for players, including test date and various performance metrics.

- **data/biometrics.csv**: Holds biometric measurement data for players, including date, height, weight, ACL, mass, MME, BMI, PGC, AEC_Act, protein, and minerals.

- **scripts/insert_data.py**: Python script for inserting new player data into the database from the CSV files.

- **scripts/update_data.py**: Python script for managing updates to existing player data, physical test results, or biometric measurements from the CSV files.

- **sql/create_tables.sql**: SQL script containing commands to create the three tables (data_player, physical_test, and biometric) in the MySQL database.

- **sql/insert_initial_data.sql**: SQL script with commands to insert initial data into the tables after creation.

- **requirements.txt**: Lists the Python package dependencies required for the project, such as libraries for database interaction and CSV processing.

## Setup Instructions
1. Ensure you have MySQL installed and running.
2. Create a new database named `Borregos_FBA`.
3. Run the `sql/create_tables.sql` script to create the necessary tables.
4. Use the `sql/insert_initial_data.sql` script to populate the tables with initial data.
5. Install required Python packages listed in `requirements.txt`.
6. Use the provided Python scripts to manage player data and updates.

## Usage
- Use `insert_data.py` to add new players and their test results.
- Use `update_data.py` to update existing player information or test results.

## Future Enhancements
Additional tables and features may be added as the project evolves to accommodate more data and functionality.