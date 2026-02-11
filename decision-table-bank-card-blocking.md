## Conditions

1. 3 incorrect PIN attempts
2. Suspicious country
3. Suspicious amount (>100 000)

## Rules

- If PIN incorrect 3 times → Card blocked
- If country and amount suspicious → Card blocked
- If only country suspicious → SMS verification
- If only amount suspicious → SMS verification
- Otherwise → Operation allowed

## Decision Table

| # | 3 incorrect PIN | Suspicious country | Suspicious amount | Result |
|---|-----------------|-------------------|------------------|--------|
| 1 | Yes | Yes | Yes | Card blocked |
| 2 | Yes | Yes | No | Card blocked |
| 3 | Yes | No | Yes | Card blocked |
| 4 | Yes | No | No | Card blocked |
| 5 | No | Yes | Yes | Card blocked |
| 6 | No | Yes | No | SMS verification |
| 7 | No | No | Yes | SMS verification |
| 8 | No | No | No | Operation allowed |
