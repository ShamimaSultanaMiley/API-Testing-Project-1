# Content    
- [ Description](#discription )
- [Summary](#summary) 
- [Newman Report](#newmanreport) 
# Description 
I have completed API testing on a booking website. The following website is the website I have tested. https://restful-booker.herokuapp.com/

Tasks Done

-CRUD operations such as Create, Get, Put & Patch, and Delete.

-Writing pre-request scripts using dynamic parameters

-API Request & Response Chaining

-Writing test scripts for data validation.

-Newman HTML & HTML Extra Report

# Summary 
The summary of all the tasks done for the restful-booker websites is given below with a table.
![Summary image](Image/report_table.JPG)

# Newman Report
The Report of all the tasks done for the restful-booker websites is given below with a table.

![Newman Report](Image/newman_report.JPG)

## Prerequisites

Before running the tests and generating HTML reports, ensure you have the following prerequisites installed on your system:

- [Postman](https://www.postman.com/downloads/): Install Postman to create and export your collection and environment files.
- [Newman](https://learning.postman.com/docs/running-collections/using-newman-cli/installation-postman-pm/): Install Newman to run Postman collections from the command line.
- [Node.js](https://nodejs.org/): Ensure you have Node.js installed, as Newman requires it.

## Instructions

Follow these steps to run your API tests and generate HTML reports using Newman and the provided collection and environment files:
1. **Clone the Repository**:
   - Clone this Git repository to your local machine using the following command:
     ```bash
     git clone https://github.com/ShamimaSultanaMiley/API-Testing-Project-1.git
     ```
2. **Navigate to the Repository Directory**:
   - Change your working directory to the repository's root folder:
     ```bash
     cd API-Testing-Project-1
     ```

3. **Install Newman Globally** (if not already installed):
   - Install Newman globally using npm (Node Package Manager):
     ```bash
     npm install -g newman
     ```

4. **Run Newman with Console Report**:
   - Execute your API tests using Newman by running the following command:
     ```bash
     newman run Booker_API.json -e Environment.json
     ```
     - Replace "Booker_API.json" with the actual filename of your collection file.
     - Replace "Environment.json" with the actual filename of your environment file.

5. **Generate HTML Report**:
   - If you want to generate an HTML report in addition to the console report, use the following command:
     ```bash
     newman run Booker_API.json -e Environment.json --reporters cli,html
     ```

6. **View Reports**:
   - The console report will be displayed in your terminal.
   - The HTML report (if generated) will be available in the `newman` directory located in the root of your project.

7. **Customize HTML Report (Optional)**:
   - You can further customize the appearance of the HTML report by providing a custom template.

**Example Command (with HTML Report)**

```bash
newman run Booker_API.json -e Environment.json --reporters cli,html


