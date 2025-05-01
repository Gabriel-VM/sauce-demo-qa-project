# Sauce Demo QA Test Project

Here you have a complete manual testing project for the [Sauce Demo](https://www.saucedemo.com/) online store.

The project aims to showcase the following:
- The creation of a well-structured test plan
- The execution of exploratory and scenario-based manual testing
- The identification, prioritization, and clear reporting of software bugs

---

## 📁 Project Structure

```
/
├── test-plan/
│   └── Sauce Demo Shopping Test Plan.pdf
├── bug-report/
│   └── BugReport.md
└── README.md
```

---

## 🧪 Test Coverage

The test plan includes tests for:
- Login page
- Homepage UI and functionality
- Hamburger menu options
- Product sorting and interaction
- Item details page
- Cart and checkout flows (including personal info, recap and confirmation pages)

Tests are written in BDD-style (`Given / When / Then`) for readability and potential BDD automation.

---

## 🐞 Bug Report Summary

The [Bug Report](./bug-report/BugReport.md) includes issues found while testing the application, especially using the `problem_user` test account. Each bug includes:
- Title
- Priority
- Description
- Reproduction steps
- Actual and expected results

High-priority issues include:
- Non-functional cart actions
- Session leakage between users
- Incorrect routing and broken CTAs
- Form input failure blocking checkout

---

## 👤 Test User Profiles

Tests were primarily conducted using the `problem_user` account, which simulates edge-case and negative scenarios.  
To verify the expected (intended) behavior of the application, use the `standard_user` account.

---

## 📌 Notes

This repository is intended for demonstration purposes, and all testing was done on Sauce Labs' public demo environment. The issues reported are specific to the `problem_user` scenario and serve to showcase QA analysis skills.

---

## 📧 Contact

If you'd like to know more about the project, feel free to open an issue or connect via GitHub.
