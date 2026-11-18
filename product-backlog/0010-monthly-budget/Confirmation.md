# Acceptance Criteria

The young professional should be able to:
- enter a single net monthly income in euros
- add a fixed expense with a name and an amount, picking a suggested name (e.g. rent, phone/internet, subscriptions) or typing their own, and edit or remove it afterwards
- see the total of fixed expenses, the amount left each month (income minus total) and the percentage of income taken by fixed expenses
- see the result update immediately after any change
- enter amounts in pt-PT format, e.g. "1250,50"
- find the same income and expenses still there after reloading the page on the same device

The system should:
- show a clear negative amount (e.g. "-120,00 €") when expenses exceed income, not an error
- reject empty, non-numeric or negative amounts with a clear pt-PT message next to the field
- calculate correctly: income 1 200 € with expenses 500 € + 80 € + 40 € leaves 580,00 € and 48,3 % of income spent
- round to cents and display euros in pt-PT format (e.g. "1 250,50 €")
- render and work at 320 px width, with no horizontal scrolling
- keep all data on the user's device and make no network request containing financial data
