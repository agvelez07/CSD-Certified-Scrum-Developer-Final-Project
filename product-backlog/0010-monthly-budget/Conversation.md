## 2026-11-18

**Scope:** In: the user enters one net monthly income and a list of fixed monthly expenses (name + amount, add / edit / remove), with suggested expense names (rent, utilities, transport, phone/internet, subscriptions, existing loan payments), and sees total fixed expenses, the amount left each month, and the share of income taken by fixed expenses. The data is saved on the user's device between visits. Out: variable expenses, spending categories and limits, multiple months or history, savings goals, multiple incomes, gross-to-net calculation, user accounts and cross-device sync, bank import.
**Users:** Young professional in a first job, with no prior finance knowledge; knows what lands in the bank account each month.
**Edge cases:** Expenses greater than income (show a clear negative "left" amount, not an error); no expenses entered; income empty, zero or negative; non-numeric input; pt-PT number format with comma decimals (e.g. 1 250,50 €); very large values; rounding to cents; browser storage empty or cleared.
**Constraints:** Net income typed by hand. Data stays on the user's device, nothing sent to a server (DoD: personal financial data never exposed). Content in clear pt-PT, euro formatting, usable at 320px width. No external API, so no integration tests needed here.
**Decisions:** Product owner wanted gross-to-net calculation and saving to an account; both were split into their own backlog items (gross-to-net salary, account and sync) so this item stays a small first slice. Suggested expense names: yes.
**Open questions:** None.
