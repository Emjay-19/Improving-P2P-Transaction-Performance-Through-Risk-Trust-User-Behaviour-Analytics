# Improving-P2P-Transaction-Performance-Through-Risk-Trust-User-Behaviour-Analytics  

## Project Overview  

P2P Transaction & Trust Analytics is a Power BI analytics project focused on understanding transaction performance, risk, disputes, user trust, and repeat usage within a peer-to-peer escrow marketplace.  

The analysis follows the complete transaction journey from transaction creation to funds release, while also examining the factors associated with failed transactions, disputes, financial losses, user trust, and customer retention.  

The project consists of three interconnected dashboards:  

1. Transaction Experience  

Examines how transactions move through the transaction lifecycle and identifies where transactions fail, are cancelled, delayed, or successfully completed.  

2. Risk & Disputes  

Analyses fraud risk, disputes, refunds, transaction losses, dispute drivers, and geographical patterns associated with financial leakage.  

3. User Trust & Retention  

Explores user verification, trust scores, transaction activity, repeat usage, and behaviours associated with continued engagement.  

Note: This is a fictional/synthetic case study created for portfolio and analytical demonstration purposes. The figures do not represent actual performance of any real company.  

## Problem Statement  

A P2P escrow platform can process thousands of transactions while still experiencing significant losses through failed transactions, cancellations, disputes, refunds, fraud risk, and poor user retention.  

Looking only at total transaction volume or transaction value does not explain why transactions fail or what behaviours contribute to successful and repeat usage.  

This project was therefore designed to answer three key areas:  

- Where are users dropping off during the transaction journey?  
- What behaviours and transaction characteristics are associated with risk, disputes, and financial losses?  
- What user behaviours are associated with trust and repeat usage?  

The goal is to transform transaction and user data into actionable insights that can support better transaction experiences, risk management, dispute reduction, and customer retention.  

## Business Questions Answered  
**Transaction Experience**  
- How many transactions successfully move through each stage of the transaction journey?  
- Where do the largest transaction drop-offs occur?  
- What is the overall transaction success rate?  
- How do cancellation and payment failure affect transaction performance?  
- How does transaction performance change over time?  
- Which user types experience better or worse transaction outcomes?  
- What is the average time required to complete a transaction?  
- Which transaction statuses account for the largest volumes?

**Risk & Disputes**    
- How many transactions result in disputes?  
- How does the dispute rate change over time?  
- Which verification groups are associated with disputes and fraud risk?  
- What are the most common reasons for disputes?  
- Which transaction risk bands show higher dispute rates?  
- Where is the highest transaction value being lost?  
- Which countries contribute most to financial losses?  
- How much value is associated with refunds and disputed transactions?  

**User Trust & Retention**  
- Does trust level influence repeat usage?
- How many users return after their initial transaction?
- What does a typical repeat user look like?
- Do verified users engage more than unverified or pending users?
- How does transaction activity differ across user groups?
- Which user behaviours are associated with successful repeat usage?
- What is the relationship between user trust and transaction activity?

## Data Source  

The project uses a synthetic dataset created to simulate transaction and user activity within a P2P escrow marketplace.  

The dataset represents approximately:  

- 12,000 transactions  
- 3,500 users  
- 62,000+ transaction events  
- Multiple transaction stages  
- User verification information  
- Transaction statuses  
- Dispute and refund information  
- Fraud-risk indicators  
- Trust scores  
- Transaction values  
- Countries and transaction categories  
- Payment methods  
- User types and activity levels

The dataset was designed specifically to demonstrate how transaction, risk, and behavioural data can be combined to answer practical business questions.

Tools and Methodology
Tools
Power BI – Data modelling, DAX calculations, visualisation and dashboard development
Power Query – Data cleaning and transformation
DAX – KPI calculations, ratios, YoY analysis and analytical measures
Excel/CSV – Dataset preparation and initial data inspection
Methodology

The analysis followed these main steps:

1. Data Preparation

The data was reviewed for consistency, relevant fields were identified, and transaction and user information were structured for analysis.

2. Data Transformation

Power Query was used to clean and transform the dataset, including date preparation, categorical fields, transaction statuses, user groups and analytical classifications.

3. Data Modelling

A structured model was created around transaction, transaction-event, user and calendar information to support analysis across different dimensions.

4. Transaction Funnel Analysis  

Transaction IDs were tracked across the six-stage lifecycle to identify conversion and drop-off points.  

5. Risk & Dispute Analysis  

Disputes, fraud-risk transactions, refunds and lost transaction value were analyzed across verification status, risk bands, dispute reasons and countries.  

6. User Behaviour Analysis  

User activity, trust scores, verification status, transaction frequency and repeat usage were compared to identify behavioural patterns associated with retention.  

7. Dashboard Development  

Three dashboards were developed with interactive filters for dimensions such as:  

Year  
Category  
Payment Method  
Country  
User Type  
Verification Status  
Fraud Risk Band  

The dashboards were designed around business questions rather than simply presenting charts, making the analysis easier to interpret and act upon.  

## Key Insights  
1. Transaction Experience  
The platform recorded 12,000 transactions with a total transaction value of approximately ₦741.95bn.  
The overall transaction success rate was 65.90%, meaning roughly one-third of transactions did not reach successful completion.  
The transaction funnel shows a major drop between Payment Confirmed (10,191) and Delivery Marked (9,575), followed by another significant drop before funds were released.  
7,908 transactions reached the released stage, representing the largest completed transaction group.  
1,212 transactions were cancelled, while 956 were disputed, 711 refunded, 616 remained pending, and 597 failed at payment.
Average transaction completion time was approximately 22 hours.  
Transaction performance varied across user types, with buyers recording the highest success rate at 67.14% compared with sellers at 66.58% and both-user transactions at 64.03%.  
Business implication  

The transaction funnel suggests that improving the stages between payment confirmation, delivery confirmation and final release could have a meaningful impact on overall transaction completion.  

2. Risk & Disputes  
There were 956 disputed transactions, representing a 7.97% dispute rate.  
615 transactions were classified as fraud-risk transactions.  
The refund rate stood at 5.93%.  
Total identified lost transaction value was approximately ₦27.89bn.  
The leading dispute categories were:  
Buyer issue – 196  
Seller issue – 194  
Payment issue – 191  
Item not received – 190  
Item not as described – 185  
Verification status also showed differences in dispute patterns. Unverified users had the highest dispute rate at 8.42%, compared with 7.90% for verified users and 7.75% for pending users.  
The highest reported transaction losses came from Ghana, South Africa, the United Kingdom, the United States, Kenya and Nigeria.  
Business implication  

Disputes are not driven by one single issue. Buyer/seller problems, payment issues and fulfilment-related complaints all contribute to transaction risk, suggesting the need for intervention across the entire transaction journey.  

3. User Trust & Retention  
The analysis identified 3,386 active users.  
2,999 users were classified as repeat users.  
Repeat usage rate was 88.57%.  
Users averaged 3.54 transactions per user.  
Average trust score was 69.46.  
Of the active users:  
2,072 were repeat users  
927 were highly active users  
387 were one-time users  
Verified users accounted for the largest number of repeat users, with 1,797 verified repeat users, compared with 626 pending and 576 unverified.  
Trust and repeat usage did not show a simple linear relationship. Some moderate trust groups demonstrated stronger repeat activity than higher trust groups.  
Business implication  

Verification appears to be an important part of the user experience, but trust alone does not completely explain retention. Transaction experience, activity levels and other behavioural factors should also be considered.  

## Recommendations  
1. Improve the transaction funnel  

Focus on the stages with the largest drop-offs, particularly the movement from payment confirmation through delivery confirmation and final fund release.  

Possible actions include:  

Automated reminders for incomplete transactions  
Clearer delivery and confirmation instructions  
Notifications when transactions remain inactive  
Monitoring unusually long completion times  
2. Reduce cancellation and payment failures  

Investigate the major reasons behind cancelled and failed transactions.  

The platform could monitor:  

Payment failure patterns  
Payment methods with higher failure rates  
Transaction categories with high cancellation rates  
User groups with repeated failed transactions  
3. Strengthen dispute prevention  

The leading dispute reasons should be incorporated into preventive measures.  

For example:  

Improve transaction descriptions  
Provide clearer buyer/seller expectations  
Strengthen delivery confirmation processes  
Monitor repeated dispute patterns  
Improve communication around payment-related issues  
4. Prioritise high-risk transactions  

Fraud-risk transactions should be monitored using behavioural and transaction-level signals such as:  

Transaction frequency  
Transaction value  
Cancellation behaviour  
Previous disputes  
Verification status  
Unusual transaction patterns  

Higher-risk transactions can receive additional verification or review before funds are released.  

5. Investigate major sources of financial loss  

The countries with the highest lost transaction value should receive deeper investigation to determine whether the losses are driven by:  

Higher transaction volumes  
Higher dispute rates  
Fraud  
Refunds  
Transaction values  
Operational issues  
6. Strengthen user retention  

Since repeat users form a significant portion of active users, the platform should identify and replicate the behaviours associated with successful repeat usage.  

Potential areas include:  

Improving the first transaction experience  
Encouraging user verification  
Reducing transaction friction  
Improving trust and reputation signals  
Personalised engagement for inactive users  
**7. Monitor trust beyond a single score**  

Trust should not be treated as a standalone retention metric. It should be analyzed alongside verification, transaction frequency, disputes, cancellations and transaction value to understand what actually drives long-term engagement.  

## Limitations  
- The dataset is synthetic and does not represent actual platform performance.  
- The analysis shows relationships and patterns but does not establish causal relationships.  
- Fraud-risk classifications are simulated and may not reflect a production fraud-detection model.  
- The analysis does not include qualitative information such as user interviews or customer support conversations.  
- Financial losses are represented within the synthetic dataset and should not be interpreted as real monetary losses.  
- Some behavioural patterns may change when tested against a larger and more representative production dataset.  
- The dashboards provide descriptive and diagnostic analytics rather than predictive fraud or churn models.  

## Conclusion  

The P2P Transaction & Trust Analytics project demonstrates how transaction, risk and user behaviour data can be combined to understand the health of a P2P escrow marketplace.  

The analysis shows that transaction volume alone is not enough to measure platform performance. A platform can process substantial transaction value while still experiencing significant losses through cancellations, disputes, refunds and failed transactions.  

The three dashboards provide a connected view of the business:  

**Transaction Experience → Risk & Disputes → User Trust & Retention**  

Together, they help identify where transactions fail, what contributes to risk and financial loss, and which user behaviours are associated with continued engagement.  

The key takeaway is that analytics should move beyond reporting what happened to helping decision-makers understand why it happened and what should be done next.  
The transaction journey was modelled across the following stages:

Created → Payment Attempted → Payment Confirmed → Delivery Marked → Buyer Confirmed → Funds Released
