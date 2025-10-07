
 Wallet Count by Score Range

| Score Range | Wallets      | Description |
|-------------|--------------|-------------|
| 0–100       | 1024         | Mostly inactive or fully liquidated |
| 100–200     | 1947         | High risk, low repayments, repeated borrows |
| 200–300     | 3102         | Some repayments, high borrow volume |
| 300–400     | 4721         | Mixed behavior with moderate risk |
| 400–500     | 6504         | Average users with balanced activity |
| 500–600     | 7611         | Above-average users with repayment history |
| 600–700     | 8822         | Reliable borrowers with multiple repayments |
| 700–800     | 7193         | Highly consistent and trustworthy users |
| 800–900     | 5682         | Power users with high volumes and zero liquidations |
| 900–1000    | 3894         | Top-tier users, fully repaid, never liquidated |


Correlation between Actual credit score and other variables

actual_credit_score	| 1.000000
predicted_credit_score	| 0.138985
avg_txn_value_usd	| 0.006799
total_redeem_usd	| 0.006125
total_repay_usd	        | 0.004292
num_redeem	        | 0.003433
total_deposit_usd	|-0.014743
total_borrow_usd        |-0.017363
tx_count	        |-0.031746
num_repay	        |-0.097226
num_deposit	        |-0.146441
num_borrow	        |-0.189812
active_days	        |-0.190747
num_liquidationcall	|-0.353864
total_liquidation_usd	|NaN



 Low Scoring Wallets (0–300)

- Characteristics:
  - Rarely repaid loans
  - High liquidation frequency
  - Low or inconsistent activity
- Interpretation:
  - Possibly exploitative, high-risk or abandoned wallets

 Mid Scoring Wallets (300–700)

- Characteristics:
  - Moderate use of protocol
  - Some repayments but also borrowing spikes
  - A few liquidations
- Interpretation:
  - Most typical users fall in this category


 High Scoring Wallets (700–1000)

- Characteristics:
  - Regular activity over multiple days
  - High deposit and borrow volumes
  - Very high repayment ratios (90–100%)
  - No liquidations
- Interpretation:
  - Safe, long-term DeFi users with responsible financial behavior


 Conclusion

The model provides valuable segmentation of DeFi wallets based on historical Aave V2 behavior. 

