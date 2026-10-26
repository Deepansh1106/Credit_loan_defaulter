# Research findings (runtime-bounded tuning stage)

Fixed-stage shortlist was selected from verified fixed five-fold results: Random Forest + SMOTE was the AP leader; XGBoost + Original was selected as a strong different-family AP configuration; LightGBM + RandomUnderSampler was the ROC-AUC leader.

A one-fold full-development XGBoost pilot with 20 trees took 1.40 seconds. Therefore, two-candidate five-fold tuning completed for XGBoost + Original and LightGBM + RandomUnderSampler using AP as refit metric. Random Forest + SMOTE tuning has not been launched: its fixed five-fold SMOTE run required about 611 seconds, exceeding the runtime-bound stage budget.

No test data were used for tuning or selection. PR/ROC curves, threshold selection, and final test evaluation remain pending until a final selection policy is resolved with the incomplete AP-leading Random Forest tuning explicitly considered.
