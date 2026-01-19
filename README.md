# Budget Calculator

A personal finance budgeting app for planning annual income, expenses, and savings with automatic calculations across annual, monthly, and per-paycheck views.

## Overview

This tool helps you create and compare different budget scenarios to optimize your financial planning. Based on a traditional spreadsheet budgeting approach, it provides automatic calculations and visual insights into your financial allocation.

## Features

✅ **Three-Column View** - See your budget across Annual, Monthly, and Per Paycheck (semi-monthly)  
✅ **Comprehensive Categories** - Track income, taxes, insurance, savings, and expenses  
✅ **Auto-Calculations** - Type in annual amounts, monthly and per-paycheck auto-calculate  
✅ **Multiple Budget Scenarios** - Create unlimited budget versions to compare different plans  
✅ **Contribution Limits** - Built-in 2026 IRS limits for 401K ($24,500), Roth IRA ($7,500), and HSA ($4,400)  
✅ **Visual Analytics** - Bar charts showing income allocation, expense breakdown, and savings breakdown  
✅ **Savings Rate Tracking** - Automatically calculates your savings rate percentage  
✅ **Budget Comparison** - Duplicate budgets and adjust to see different financial scenarios  

## Quick Start

### Option 1: Open Directly

Simply open `index.html` in your browser - no build step required!

```bash
# Clone the repository
git clone https://github.com/rservais/budget_calculator.git
cd budget_calculator

# Open in browser (macOS)
open index.html

# Or just double-click index.html in your file explorer
```

### Option 2: Serve Locally

```bash
# Using Python
python -m http.server 8000

# Using Node.js
npx serve

# Then visit http://localhost:8000
```

## Usage

### Creating Your First Budget

1. The app opens with a sample "Conservative Plan" budget
2. Click into any **Annual** field and enter your numbers
3. **Monthly** and **Per Paycheck** columns auto-calculate
4. Add notes in the rightmost column for each line item

### Budget Categories

**Income**
- Gross Income - Your total annual income before deductions

**Taxes + Insurance**
- Taxes - Federal, state, and local taxes
- Insurance - Health, dental, vision insurance premiums

**Savings**
- 401K - Up to $24,500 (2026 limit)
- Roth IRA - Up to $7,500 (2026 limit)
- HSA - Up to $4,400 (2026 limit)
- HYSA - High-yield savings account
- Brokerage - Taxable investment account

**Expenses**
- Rent (fixed) - Monthly rent or mortgage
- Living Expenses - Utilities, groceries, gas, etc.
- Travel Fund - Vacation and travel budget
- Discretionary - Entertainment, dining out, shopping

### Key Metrics

The app automatically calculates:
- **Total Tax + Insurance** - Total deductions
- **Total Savings** - Total retirement and savings contributions
- **Total Expenses** - Total spending
- **Subtotal Budgeted** - Sum of all allocations
- **Remaining Income** - Money left over (green = surplus, red = deficit)
- **Savings Rate** - Percentage of income going to savings

### Creating Multiple Budget Scenarios

1. Click **"New Budget"** to create a fresh scenario
2. Or **hover over an existing budget tab** and click the duplicate icon
3. Switch between budgets using the tabs
4. Compare different scenarios side-by-side by duplicating your browser tab

### Visualizations

Click the **"Visualizations"** tab to see:
- Income allocation breakdown (Taxes vs Savings vs Expenses)
- Detailed expense breakdown by category
- Detailed savings breakdown by account type
- Percentage of income for each major category

## Budget Strategy Tips

**50/30/20 Rule Baseline:**
- 50% Needs (rent, utilities, groceries)
- 30% Wants (dining, entertainment, travel)
- 20% Savings (retirement, emergency fund)

**Aggressive Savings:**
- Maximize 401K to IRS limit ($24,500)
- Max out Roth IRA ($7,500)
- Max out HSA if eligible ($4,400)
- Target 40%+ savings rate

**Conservative Approach:**
- 10-15% to 401K (especially if employer match)
- Build 3-6 month emergency fund in HYSA
- Target 20-25% savings rate

## Technology Stack

- **React 18** - UI framework
- **Tailwind CSS** - Styling
- **Vanilla JavaScript** - No build process required
- **Self-contained** - Single HTML file, no dependencies

## Project Structure

```
budget_calculator/
├── index.html          # Complete application
├── README.md           # This file
└── .gitignore         # Git ignore rules
```

## Data Persistence

Currently, budgets are stored in browser memory and reset on page refresh. For persistent storage, you could:
- Add browser localStorage
- Export/import JSON files
- Connect to a backend database
- Use Google Sheets integration

## Future Enhancements

- [ ] Expense tracking - Enter actual monthly spending vs budget
- [ ] Month-by-month tracking throughout the year
- [ ] Historical comparison across years
- [ ] Export to PDF/CSV
- [ ] Import from bank statements
- [ ] Budget vs actual variance reporting
- [ ] Goal tracking (emergency fund, down payment, etc.)
- [ ] Net worth tracking
- [ ] Investment portfolio allocation

## Contributing

This is a personal finance tool. Feel free to fork and customize for your own needs!

## License

MIT License - use and modify as needed.

## Contact

Built by Ryan Servais for personal budgeting and financial planning.

---

## Sample Budget Scenarios

### Scenario 1: Aggressive Savings (40% savings rate)
- Income: $120,000
- 401K: $24,500 (max)
- Roth IRA: $7,500 (max)
- HSA: $4,400 (max)
- Additional Savings: $11,600
- Target: Build wealth rapidly, retire early

### Scenario 2: Balanced Approach (25% savings rate)
- Income: $120,000
- 401K: $18,000 (15%)
- Roth IRA: $7,500 (max)
- Emergency Fund: $4,500
- Target: Comfortable retirement, lifestyle balance

### Scenario 3: Debt Payoff Focus (15% savings + extra to debt)
- Income: $120,000
- 401K: $6,000 (employer match only)
- Emergency Fund: $2,000
- Extra to Debt: $24,000
- Target: Eliminate debt, then boost savings

Use the app to model your own scenarios!
