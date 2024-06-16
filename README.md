# Business Management System - Web Development Project #2

This project is a Business Management System developed as part of the course IS601 Mini Project 3 at New Jersey Institute of Technology. The system allows for the management of companies and employees, including creating, reading, updating, and deleting (CRUD) operations. It also supports the import of data via CSV files. The project is implemented using Python and Flask and includes a robust test suite to ensure functionality.

### Features
- CRUD operations for Companies and Employees.
- Import data from CSV files.
- Search and filter functionality for Companies and Employees.
- Deployed using Heroku with separate environments for development and production.
- Robust exception handling and error messages for invalid inputs.
### Installation
- git clone https://github.com/Anu0408/business-management-system.git
- cd business-management-system
- python3 -m venv venv
- source venv\Scripts\activate  #On Windows
#### Install the required packages:
- pip install -r requirements.txt
#### Set up the database:
- Copy the .env file from the flask_sample into the BusinessManagement folder.
#### Initialize the database by running the provided SQL script:
- python BusinessManagement/sql/init_db.py
### Usage
#### Running the Application
1. Start the Flask application: flask run
2. Access the application: Open your web browser and navigate to http://127.0.0.1:5000.

### Adding Data
1. Adding a Company: Navigate to the "Add Company" page, fill in the required details, and submit the form.
2. Adding an Employee: Navigate to the "Add Employee" page, fill in the required details, and submit the form.
#### Importing Data from CSV
- Select the data.csv file from /import route of the application and upload it.
#### Testing
Run the test cases individually to save on query quota usage:
- pytest BusinessManagement/test/name_of_test.py -rA

### Deployment
#### Heroku Deployment
##### Create new dynos/VMs in Heroku:
Create and push new branches:
- git checkout dev
- git pull
- git checkout -b mp3-prod
- git push origin mp3-prod
- git checkout -b mp3-dev
- git push origin mp3-dev
- git checkout -b MiniProject-3

- git add .
- git commit -m "Add baseline files"
- git push origin MiniProject-3

### License
This project is licensed under the MIT License. See the LICENSE file for details.
