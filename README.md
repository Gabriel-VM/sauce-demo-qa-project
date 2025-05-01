# Sauce Demo QA Test Project

This repository documents a complete manual testing project for the [Sauce Demo](https://www.saucedemo.com/) online store.

The objective is to showcase the ability to:
- Create a well-structured test plan
- Perform exploratory and scenario-based manual testing
- Identify, prioritize, and report software bugs in a clear, professional format

---

## 📁 Project Structure

```
/
├── test-plan/
│   └── SauceDemoTestPlan.pdf
├── bug-report/
│   └── BugReport.md
├── evidences/             # (optional, for screenshots or videos)
│   └── [bug-screenshots]
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

Tests were run using various predefined user accounts provided by Sauce Demo, with special focus on `problem_user`, which simulates edge-case behavior for negative testing.

---

## 📌 Notes

This repository is intended for demonstration purposes, and all testing was done on Sauce Labs' public demo environment. The issues reported are specific to the `problem_user` scenario and serve to showcase QA analysis skills.

---

## 📧 Contact

If you'd like to know more about the project, feel free to open an issue or connect via GitHub.