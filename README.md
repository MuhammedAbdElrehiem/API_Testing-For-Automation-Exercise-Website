Postman Automated Testing for API
=================================

Overview
--------

This project implements a comprehensive suite of automated API tests for the Automation Exercise website using Postman and Newman. The tests ensure the functionality, reliability, and performance of various API endpoints, including user account creation, product search, and login verification.

Table of Contents
-----------------

-   [Features](#features)
-   [Technologies Used](#technologies-used)
-   [Getting Started](#getting-started)
-   [How to Run Tests](#how-to-run-tests)
-   [Continuous Integration](#continuous-integration)
-   [Contributing](#contributing)
-   [License](#license)

Features
--------

-   Automated tests for key API endpoints, including:
    -   User account creation
    -   User login
    -   Product search
    -   Account deletion
    -   User account updates
-   Detailed HTML reports generated using Newman.
-   Integration with GitHub for version control.

Technologies Used
-----------------

-   **Postman**: For creating and managing API requests and test cases.
-   **Newman**: Command-line tool for running Postman collections.
-   **Jenkins**: For continuous integration and automating test execution.
-   **Git**: For version control and collaboration.

Getting Started
---------------

To get a local copy of this project up and running, follow these steps:

1.  **Clone the repository**

    bash

    Copy code

    `git clone https://github.com/MuhammedAbdElrehiem/API_Testing-For-Automation-Exercise-Website.git`

2.  **Navigate to the project directory**

    bash

    Copy code

    `cd API_Testing-For-Automation-Exercise-Website`

3.  **Install Newman** Ensure you have Node.js installed, then install Newman globally:

    bash

    Copy code

    `npm install -g newman`

4.  **Run the Postman tests** Execute the following command to run the tests:

    bash

    Copy code

    `newman run <your_postman_collection.json> -e <your_environment.json> -r html`

How to Run Tests
----------------

1.  Open your terminal and navigate to the project directory.
2.  Run the following command to execute the test suite:

    bash

    Copy code

    `newman run collection.json -r html`

3.  After running the tests, an HTML report will be generated in the project directory.

Continuous Integration
----------------------

This project uses Jenkins to automate the execution of tests upon code commits. When a new release is pushed to the GitHub repository, Jenkins triggers the test suite and generates an updated HTML report.

### Setting up Jenkins

1.  Install Jenkins on your local machine or server.
2.  Create a new freestyle project in Jenkins.
3.  Configure the Git repository and set up build triggers for GitHub webhooks.
4.  Add build steps to execute the Newman tests and archive the generated HTML report.

Contributing
------------

Contributions are welcome! If you have suggestions or improvements, please fork the repository and submit a pull request.

License
-------

This project is licensed under the MIT License - see the LICENSE file for details.
