# Part C — Questions, Assumptions & Contradictions

## 1. Questions

1. Can an employee work at multiple branches? (SRS 7.2)
2. Can one reservation result in multiple rentals? (SRS 7.11–7.12)
3. Can a rental have multiple insurance packages? (SRS 7.13)

## 2. Assumptions

1. Each employee belongs to one branch at a time. (SRS 7.2)
2. Each reservation can create only one rental. (SRS 7.12)

---

# Part D — Business Rules Beyond Constraints

| # | SRS Section | Business Rule | Why Constraints Are Not Enough | How to Enforce It |
|---|---|---|---|---|
| 1 | 7.7 | A blacklisted customer cannot make a new reservation. | The system must check the customer's blacklist status before creating a reservation. | Application Logic: Check whether the customer is blacklisted before allowing a reservation to be created. |