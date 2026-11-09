# UI Application Automation Tests

This project contains a suite of automated UI tests developed for the [UI Course Test Application](https://nikita-filonov.github.io/qa-automation-engineer-ui-course/#/auth/login).

The automation framework was built from scratch using **Python**, **Pytest**, **Playwright** and **Allure**.

## Project Overview

The project focuses on testing the application's core functionality, including user registration, authentication, course management and dashboard interactions.

The tests are organized using the Page Object Model (POM) design pattern, with reusable components and fixtures to improve maintainability and reduce code duplication.

The test application is publicly available at [GitHub](https://github.com/Nikita-Filonov/qa-automation-engineer-ui-course).

## Getting Started

### Clone the Repository

To get started, clone the project repository using Git:

```bash
git clone https://github.com/neverw1nter77/autotests-ui.git
cd autotests-ui
```

### Create a Virtual Environment

It's recommended to use a virtual environment to manage project dependencies. Follow the instructions for your operating
system:

#### Linux / MacOS

```bash
python3 -m venv venv
source venv/bin/activate
```

#### Windows

```bash
python -m venv venv
venv\Scripts\activate
```

### Install Dependencies

Once the virtual environment is activated, install the project dependencies listed in `requirements.txt`:

```bash
pip install -r requirements.txt
```

### Additional Playwright Setup (if needed)

If you're running Playwright for the first time, you might need to install the required browsers:

```bash
playwright install
```

### Running the Tests with Allure Report Generation

To run the tests and generate an Allure report, use the following command:

```bash
pytest -m "regression" --alluredir=./allure-results
```

This will execute all tests in the project and display the results in the terminal.

### Viewing the Allure Report

After the tests have been executed, you can generate and view the Allure report with:

```bash
allure serve allure-results
```

This command will open the Allure report in your default web browser.
