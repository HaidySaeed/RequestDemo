## 📁 Project Structure

```text
# SIFI Playwright Automation Framework

This project is an end-to-end test automation framework built using **Playwright + TypeScript** for testing the **SIFI Request a demo**.

---

## Tech Stack
- Playwright
- TypeScript
- Page Object Model (POM)
- Node.js

## Project Structure

SIFI/
│
├── pages/
│   ├── formPage.ts        # Get Started form page (inputs, dropdowns, submit)
│   ├── optionsPage.ts     # Select option page (Fast-track / Request call)
│   ├── bookDemo.ts        # Book demo & timeslot page
│   └── POManager.ts       # Central Page Object Manager
│
├── tests/
│   └── requestDemo.spec.ts # End-to-end test scenario
│
├── utils/
│   └── testData.ts        # Test data (user info + dropdown values)
│
├── playwright.config.ts
├── package.json
├── README.md
└── .gitignore
```

##  Test Scenario Covered
- Open SIFI Get Started page
- Accept cookies if shown
- Switch to English (if visible)
- Fill Get Started form
- Select dropdown values (Job, Industry, Size)
- Submit form
- Choose **Fast-track onboarding**
- Select demo option
- Book a demo

  ##  How to Run the Tests

1. **Clone the repository**  
```bash
git clone https://github.com/HaidySaeed/SIFI.git
cd SIFI
```

2. **Install dependencies**  
```bash
npm install
```

3. **Install Playwright browsers**  
```bash
npx playwright install
```

4. **Run tests in headed mode (browser visible)**  
```bash
npx playwright test --headed
```

5. **Run tests in headless mode (default)**  
```bash
npx playwright test
```





