# Auto Ticket Classification using Flow Designer

## 📌 Project Overview

The **Auto Ticket Classification using Flow Designer** project is a ServiceNow-based automation solution designed to simplify and automate the classification of IT support tickets in a school environment.

The school IT helpdesk receives multiple support requests from students and teachers related to issues such as **WiFi connectivity, hardware problems, password/login issues, and slow computers**. Normally, IT staff need to manually identify the issue and select the appropriate category and subcategory.

This project automates that process using **ServiceNow Flow Designer**, allowing tickets to be classified automatically based on keywords present in the **Short Description**.

---

## 🎯 Problem Statement

IT support staff spend considerable time manually reviewing and categorizing support tickets.

The manual process can lead to:

* Increased workload for IT staff
* Incorrect ticket categorization
* Inconsistent classification
* Delayed ticket processing
* Difficulty handling a large number of requests

The project addresses these issues by automatically identifying the ticket type and assigning the appropriate category and subcategory.

---

## 💡 Proposed Solution

When a student creates a support ticket, they only need to provide:

* **Caller Name**
* **Short Description**

The student does not need to manually select the Category or Subcategory.

After the ticket is submitted, **Flow Designer** checks the Short Description for predefined keywords and automatically updates the ticket with the corresponding Category and Subcategory.

---

## ⚙️ Automation Logic

| Keyword / Description | Category    | Subcategory     |
| --------------------- | ----------- | --------------- |
| WiFi                  | Network     | WiFi            |
| Projector             | Hardware    | Projector       |
| Password / Login      | Access      | Forgot Password |
| Slow / Hanging        | Performance | Slow Computer   |

### Example

If a student enters:

> "My laptop is slow and keeps hanging."

The Flow Designer identifies the keywords **Slow** or **Hanging** and automatically sets:

**Category:** Performance
**Subcategory:** Slow Computer

---

## 🔄 Workflow

```text
Student Creates Ticket
        ↓
Enter Caller Name
        ↓
Enter Short Description
        ↓
Submit Ticket
        ↓
Flow Designer Triggered
        ↓
Analyze Short Description
        ↓
Identify Predefined Keyword
        ↓
Assign Category
        ↓
Assign Subcategory
        ↓
Ticket Classified Automatically
```

---

## 🛠️ Technologies Used

* **ServiceNow**
* **Flow Designer**
* **ServiceNow Tables**
* **Choice Fields**
* **Business Process Automation**
* **No-Code Automation**

---

## ✨ Key Features

* Automatic ticket classification
* Keyword-based classification
* Automatic Category assignment
* Automatic Subcategory assignment
* No-code implementation using Flow Designer
* Reduced manual effort
* Consistent ticket classification
* Improved data accuracy
* Easy maintenance and scalability
* Suitable for educational IT helpdesks

---

## 🔐 Security and Validation

The project follows basic security and access-control practices to ensure that ticket information can only be accessed or modified by authorized users.

Testing and validation are performed to verify:

* Correct ticket creation
* Correct keyword detection
* Correct Category assignment
* Correct Subcategory assignment
* Proper Flow Designer execution
* Data accuracy
* Appropriate user access

---

## 🧪 Testing

The automation is tested using different ticket descriptions.

| Test Case | Input                       | Expected Result             |
| --------- | --------------------------- | --------------------------- |
| TC01      | WiFi is not working         | Network → WiFi              |
| TC02      | Projector is not displaying | Hardware → Projector        |
| TC03      | Forgot my Password          | Access → Forgot Password    |
| TC04      | Unable to Login             | Access → Forgot Password    |
| TC05      | Computer is Slow            | Performance → Slow Computer |
| TC06      | System is Hanging           | Performance → Slow Computer |

---

## 📈 Benefits

### For Students

* Simple ticket creation
* No need to select technical categories
* Faster ticket submission

### For IT Staff

* Reduced manual classification
* Less repetitive work
* Consistent ticket categorization
* Improved ticket processing efficiency

### For the Organization

* Scalable helpdesk workflow
* Better data consistency
* Reduced classification errors
* Easy-to-maintain automation

---


## 📋 Project Outcome

The **Auto Ticket Classification using Flow Designer** project successfully automates the classification of school IT support tickets.

By using predefined keywords and ServiceNow Flow Designer, the system automatically assigns the appropriate Category and Subcategory without requiring manual classification by the student or IT staff.

The solution demonstrates how **ServiceNow no-code automation** can be used to create a simple, scalable, and maintainable IT helpdesk workflow.

---

## 👥 Team

**Team ID:** SWTID-2026-8426

**Project:** Auto Ticket Classification using Flow Designer

---

## 📄 License

This project was developed for educational and demonstration purposes.
