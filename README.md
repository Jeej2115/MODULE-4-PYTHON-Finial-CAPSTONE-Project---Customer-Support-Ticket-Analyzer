# MODULE-4-PYTHON-Finial-CAPSTONE-Project---Customer-Support-Ticket-Analyzer
Analyzing support tickets helps identify common customer issues, understand customer sentiment, evaluate support quality, and identify areas for improvement. The Customer Support Ticket Analyzer is a Python-based project that stores,cleans, analyzes,extracts useful insights from customer support ticket data.

# Customer Support Ticket Analysis System

## Project Overview

Customer support teams handle numerous service tickets daily. Analyzing support tickets helps identify common issues, understand customer sentiment, evaluate support quality, and identify areas for improvement.

In this project, a **Python-based Ticket Analysis System** is developed to store, clean, analyze, and extract meaningful insights from customer support tickets.

The project demonstrates how Python programming concepts can be applied to a real-world customer support scenario. The system works with ticket information such as ticket number, customer name, issue description, and priority.

---

## Objectives

The main objectives of this project are to:

* Store customer support ticket information.
* Add new tickets using user input.
* Automatically generate ticket numbers.
* Validate ticket priority levels.
* Clean and standardize issue descriptions.
* Analyze frequently used keywords.
* Perform priority-based ticket analysis.
* Identify the ticket with the longest issue description.
* Extract unique words from ticket descriptions.
* Generate useful insights from customer support data.

---

## Technologies Used

* **Python**
* **Jupyter Notebook / JupyterLab**

### Python Concepts Used

* Lists
* Dictionaries
* Sets
* `for` loops
* `while` loops
* Conditional statements
* Functions
* User input
* String manipulation

---

## Ticket Data Structure

The project stores ticket information using a **dictionary of lists**.

The main fields are:

| Field               | Description                         |
| ------------------- | ----------------------------------- |
| `Ticket_No`         | Unique ticket number                |
| `Customer_Name`     | Name of the customer                |
| `Issue_Description` | Description of the customer's issue |
| `Priority`          | Priority level of the ticket        |

The supported priority levels are:

* **High**
* **Medium**
* **Low**

---

## Project Workflow

### Step 1: Preloaded Tickets

The project starts with a set of predefined customer support tickets.

Each ticket contains:

* Ticket number
* Customer name
* Issue description
* Priority

The initial ticket data is displayed in a readable format.

---

### Step 2: Add More Tickets

The system allows users to add new customer support tickets.

The user is asked:

```text
How many new tickets do you want to add?
```

For each new ticket, the system collects:

* Customer Name
* Issue Description
* Priority

Ticket numbers are automatically assigned, starting from **11**.

The priority is validated to accept only:

```text
High
Medium
Low
```

The new ticket information is then appended to the existing `ticket_data`.

---

### Step 3: Text Cleaning for Issue Descriptions

The issue descriptions are cleaned before analysis.

The cleaning process includes:

* Removing punctuation such as `.`, `,`, `!`, `?`, and `-`
* Converting multiple spaces into a single space
* Removing leading and trailing spaces
* Converting text to lowercase
* Replacing common shorthand, such as `ok` with `okay`

Python string methods such as the following are used:

```python
.replace()
.split()
' '.join()
.strip()
.lower()
```

This ensures that the issue descriptions are standardized and easier to analyze.

---

### Step 4: Keyword-Based Issue Insights

A function is created to count tickets containing a particular word:

```python
def count_tickets_with_word(word):
```

The function performs a **case-insensitive search** across all issue descriptions.

The following keywords are analyzed:

* `poor`
* `good`
* `slow`
* `excellent`

This provides a simple way to identify frequently occurring terms and understand patterns in customer feedback.

---

### Step 5: Final Summary and Insights

The final stage provides detailed analytics from the cleaned ticket data.

The system performs the following analysis:

#### 1. Final Cleaned Ticket Data

Displays the complete cleaned `ticket_data` in a readable dictionary-of-lists format.

#### 2. Priority Analysis

Calculates the number of:

* High-priority tickets
* Medium-priority tickets
* Low-priority tickets

#### 3. Longest Issue Description

Identifies the ticket with the longest issue description based on word count.

The following details are displayed:

* Ticket number
* Customer name
* Cleaned issue description
* Word count

#### 4. Unique Words

A Python set is used to extract all unique words from the issue descriptions.

The system displays:

* Total number of unique words
* Sorted list of unique words

---

## Key Learning Outcomes

Through this project, the following Python skills are practiced:

* Creating and modifying lists
* Working with dictionaries
* Using sets to identify unique values
* Using `for` and `while` loops
* Creating and calling functions
* Using conditional statements
* Accepting user input
* Cleaning and manipulating strings
* Counting words and keywords
* Sorting data
* Extracting meaningful information from raw data

---

## Example Insights

The Ticket Analysis System can provide insights such as:

* How many tickets have High, Medium, and Low priority.
* How often keywords such as **good**, **poor**, **slow**, and **excellent** occur.
* Which ticket contains the longest issue description.
* How many unique words are present across all ticket descriptions.

These insights can help support teams identify recurring issues and understand patterns in customer support requests.

---

## How to Run the Project

1. Open **Jupyter Notebook** or **JupyterLab**.
2. Create a new Python notebook.
3. Enter the preloaded ticket data.
4. Run the project steps in the following order:

   * Step 1: Preloaded Tickets
   * Step 2: Add More Tickets
   * Step 3: Text Cleaning
   * Step 4: Keyword-Based Issue Insights
   * Step 5: Final Summary & Insights
5. Provide the required information when prompted.
6. Review the final ticket analysis and insights.

---

## Project Outcome

The project transforms raw customer support ticket information into cleaned and structured data that can be analyzed using Python. It demonstrates how basic programming and data-handling techniques can be applied to a practical customer service problem.

The system provides a foundation for further analysis, such as **sentiment analysis, issue categorization, ticket trend analysis, and data visualization**.

---

## Conclusion

The **Customer Support Ticket Analysis System** provides practical experience in using Python to store, clean, analyze, and extract insights from customer support tickets. The project combines data structures, string manipulation, loops, functions, and conditional statements to process real-world ticket information.

By completing this project, I developed a better understanding of how Python can be used for **data cleaning, keyword analysis, data organization, and extracting meaningful insights**. These skills can be applied to larger datasets and more advanced customer support analytics projects in the future.


