# AV_JanataHack_Customer_Segmentation
Repository for Analytics Vidhya Hackathon for Customer Segmentation

Public LB: 15 / 369

Approach: 
XGBoost Classifier model using Grid Search CV & Stratified K Fold with some Feature Engineering.

After analysing Train & Test Data, I've observed that almost 90% of the Test IDs are already available in Train Data & the Test Entries corresponding to those IDs are almost similar to the Train Entries.

So, I want to give more importance to those IDs and the entries. So, I've assigned Segmentations to those entries available in the Test Data and concatenated with the Train Data for Training. I included the IDs for training.

(i.e.) 
No. of Training Data Entries = 8068
No. of Test Data Entries     = 2627
No. of Test Data Entries matching Training IDs = 2332

No. of new Training Data Entries = (8068 + (2332 * X ))
where X - No. of times I want to concatenate.
