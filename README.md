# Singlish → Sinhala Transliteration Tester

> Automated negative-test suite for [pixelssuite.com/chat-translator](https://www.pixelssuite.com/chat-translator) — 50 test cases, Playwright-driven, Excel-recorded.

![Python](https://img.shields.io/badge/Python-3.11+-3fb950?style=flat-square&logo=python&logoColor=white)
![Playwright](https://img.shields.io/badge/Playwright-automation-58a6ff?style=flat-square&logo=playwright&logoColor=white)
![Tests](https://img.shields.io/badge/Test_Cases-50-bc8cff?style=flat-square)
![SLIIT](https://img.shields.io/badge/IT3040-SLIIT-ffa657?style=flat-square)

---

## Overview

Evaluates the **accuracy and reliability** of a chat-based Singlish-to-Sinhala transliteration tool via negative testing — probing edge cases and failure scenarios that expose incorrect or unexpected outputs.

**Module:** IT3040 – IT Project Management (ITPM) | Assignment 1 | SLIIT

---

## Technologies

| Technology | Purpose |
|---|---|
| `Python 3.11 / 3.12` | Core scripting language |
| `Playwright` | Browser automation framework |
| `OpenPyXL` | Excel file read / write |
| `Google Chrome / Chromium` | Browser for test execution |

---

## Installation

### Step 1 — Clone the repository

```bash
git clone <your-repo-link>
cd test_automation
```

### Step 2 — Install dependencies

```bash
pip install playwright openpyxl
```

### Step 3 — Download Playwright browsers

```bash
playwright install
```

---

## Run the test suite

```bash
python test_automation.py \
  --excel         "Assignment 1 - Test cases.xlsx" \
  --url           "https://www.pixelssuite.com/chat-translator" \
  --wait-ms       5000 \
  --type-delay-ms 80 \
  --slow-mo-ms    200 \
  --save-every    1 \
  --keep-open
```

---

## Project structure

```
test_automation/
│
├── test_automation.py               # Main automation script
├── Assignment 1 - Test cases.xlsx   # Test cases & recorded results
└── README.md                        # Project documentation
```

---

## Output columns

| Column | Description |
|---|---|
| `Actual Output` | Transliteration result captured from the tool |
| `Status` | `Pass` or `Fail` based on expected vs actual output |

---

## Important notes

> **Excel filename** must match exactly as specified in the command above.

> **Stable internet** is required throughout test execution.

> **Do not close** the browser window while tests are running.

---

## Submission checklist

- [x] Excel file completed with all 50 test cases
- [x] Automation script executed successfully
- [x] GitHub repository updated
- [x] README.md added
- [x] ZIP file submitted to CourseWeb

---

## Author

| Field | Details |
|---|---|
| **Name** | Asanka Gayan Ekanayaka |
| **Student ID** | IT23636910 |
| **Module** | IT3040 – IT Project Management |
| **Institution** | SLIIT |
