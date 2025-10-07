Project Description:

This project builds a machine learning model using TensorFlow to assign a credit score (between 0 and 1000) to Ethereum wallets based on their historical interaction with the Aave V2 DeFi protocol. The goal is to determine how responsible a wallet is based on its transaction behavior.

Workflow:

-Load raw transaction data (in JSON format).

-Engineer features for each wallet:

-deposit_count

-borrow_count

-repay_count

-liquidation_count

-total_deposited_usd

-total_borrowed_usd

-total_repaid_usd

-repay_ratio

-active_days

-Compute synthetic labels (scores between 0 and 1000) based on rules.

-Train a TensorFlow regression model to predict credit scores.

-Use the model to predict scores for all wallets.

-Save results and plot score distribution.

Features used for credit score calculation:

-Number of actions (deposits, borrows, repays, etc.)

-USD value of deposits, borrows, and repayments

-Repayment ratio (repaid/borrowed)

-Number of active days

-Liquidation frequency

Model information:

Model: Deep Neural Network using TensorFlow (ANN)

- loss: 30482.7031 - mae: 111.8217 - val_loss: 29621.9961 - val_mae: 105.0373

Outputs:

wallet_credit_scores.csv : wallet addresses with predicted scores

score_distribution.png : visualization of score distribution

analysis.txt : behavior analysis based on score bands
