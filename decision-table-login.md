## 📌 Description
Testing the login functionality using Decision Table technique.

## Conditions

1. Correct login entered
2. Correct password entered

## Possible Results

- Successful login
- Error message displayed

---

## Decision Table

| # | Correct Login | Correct Password | Result |
|---|---------------|-----------------|--------|
| 1 | Yes | Yes | Successful login |
| 2 | Yes | No | Error message |
| 3 | No | Yes | Error message |
| 4 | No | No | Error message |

---

## Coverage Explanation

There are 2 conditions with 2 possible values each (Yes/No).

Total combinations:
2 × 2 = 4

Each combination is covered with a separate test case.
