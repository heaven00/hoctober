Knoctober - Analytics Vidya
---------------------------
https://www.analyticsvidhya.com/blog/2016/10/winners-approach-codes-from-knocktober-xgboost-dominates/

Cross Validation Framework
==========================

1. Take data from 2004 - 2005 for training.
2. Validation set > 2005


Trial 1
-------

Data Processing : -

    - Split registration date into month year date
    - Generate the output column based on the favourable outcomes.
      """
      For the first 2 formats, a favourable outcome is defined as getting a health_score, while in the third format it is defined as visiting at least a stall.
      You need to predict the chances (probability) of having a favourable outcome.
      """
      Create a column with 0/1 for all patients-CampID combination.
    - Fill all Nan Registration Dates with padding.
    - Convert Months string to numeric.


Trial 2
-------

Data Processing : -

    - Use the last final transformed file.
    - Add Health Camp Categories
    - Time of the Health Camps

Trial 3
-------

Data Processing : -

    - Use trial 2 final transformed file.
    - Add Patient first interaction time split into day, month and year
    - Add City Type after filling na with 'Z' ---- Not so useful removed
    - Add Social Columns ---- FAIL

Learnings
---------

    - Check all distributions to get the most efficient CV model.
    - Note down features as soon as you think of one and try to finish well before time.
