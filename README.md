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

## Tools and Methodology  

**Tools**  
- Power BI – Data modelling, DAX calculations, visualisation and dashboard development  
- Power Query – Data cleaning and transformation  
- DAX – KPI calculations, ratios, YoY analysis and analytical measures  
- Excel/CSV – Dataset preparation and initial data inspection  

**Methodology**  
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
- Year  
- Category  
- Payment Method  
- Country  
- User Type  
- Verification Status  
- Fraud Risk Band  

The dashboards were designed around business questions rather than simply presenting charts, making the analysis easier to interpret and act upon.  

<img width="1199" height="1568" alt="image (4)" src="https://github.com/user-attachments/assets/25261688-e63b-4be2-9461-c3f9acf8372e" />


## Summary of Findings

The analysis revealed three major themes across the P2P transaction ecosystem:  

**1. Transaction completion remains a major challenge**  
The platform processed a high volume of transactions, but only **65.90% achieved successful completion**. The largest drop-offs occurred between payment confirmation, delivery confirmation and the final release of funds.  

**2. Risk and disputes are creating significant value leakage**  
The platform recorded **956 disputes, 615 fraud-risk transactions and a 5.93% refund rate,** contributing to approximately **₦27.89bn in lost transaction value**. Buyer issues, seller issues, payment problems and fulfilment-related issues were the most common dispute drivers.

**3. Strong user engagement exists, but trust alone does not explain retention**  
The platform recorded **2,999 repeat users** and an **88.57% repeat usage rate** among the analyzed active-user population. However, the relationship between trust score and repeat usage was not completely linear, suggesting that retention is influenced by more than trust alone. Verification, transaction experience and overall user activity also deserve attention.

## Key Insights  

**1. Transaction performance declined despite strong transaction volume**  
The platform processed **12,000 transactions worth ₦741.95bn**, yet the overall transaction success rate was only **65.90%**. Transaction performance also declined year-over-year, with total transactions falling by **52.8%** and transaction value falling by **45.7%**. This suggests that the challenge is not simply generating transaction activity; the platform also needs to improve the percentage of transactions that successfully progress through the complete transaction journey.  

**2. The largest transaction drop-offs occur after payment confirmation**  
The transaction funnel shows that **10,191 transactions reached payment confirmation**, but only **9,575 progressed to the delivery-marked stage**, with **7,908 eventually reaching funds release**. This indicates that transaction friction becomes more visible after payment has been confirmed, particularly around fulfilment, buyer confirmation and final release. This suggests that improving the post-payment experience could have a meaningful impact on overall transaction success.  

**3. Transaction cancellations and failures are contributing to performance leakage**  
The platform recorded **1,212 cancelled transactions** and **597 payment-failed transactions**, showing that a considerable number of transactions do not reach completion even before considering disputes and refunds. The **10.10% cancellation rate** also represents a significant source of lost transaction opportunities.  
This indicates a need to understand why users cancel transactions and whether payment, seller responsiveness, fulfilment or other friction points are responsible.  

**4. Disputes represent a significant source of financial risk**  
The platform recorded **956 disputed transactions, resulting in a 7.97% dispute rate**, while total lost transaction value reached approximately **₦27.89bn**. This means the impact of transaction problems extends beyond individual failed transactions and can translate into substantial financial leakage.  
The concentration of losses across countries also suggests that risk management may need to consider geographical differences rather than applying the same controls uniformly across all markets.  

**5. Disputes are driven by several competing problems**  
Buyer issues accounted for **196 disputes**, followed closely by seller issues **(194)**, payment issues **(191)**, items not received **(190)** and items not as described **(185)**. The relatively close distribution across these categories suggests that disputes are not being driven by one isolated problem. Instead, they appear to originate from different points within the transaction experience, including payment, communication, fulfilment and product expectations.  
This means reducing disputes will likely require improvements across the entire transaction journey rather than focusing on a single dispute category.  

**6. Unverified users show a higher dispute rate**  
Unverified users recorded an **8.42% dispute rate**, compared with **7.90%** among verified users and **7.75%** among pending users.
Although the difference is not large enough to establish verification as the sole cause of disputes, the pattern suggests that verification status may be useful as one of several risk signals when assessing transaction behaviour.  

**7. User retention is strong, but activity is declining**  
The platform recorded **2,999 repeat users** and an **88.57% repeat usage rate**, indicating strong evidence of continued engagement among users who return to the platform. However, active users declined by **35.4% year-over-year**, while repeat users declined by **65.3%**. This combination suggests that although the users who remain active show strong repeat behaviour, the overall active and returning user base is shrinking.  
The priority should therefore not only be encouraging existing users to transact repeatedly but also understanding why previously active users are no longer returning.  

**8. Trust appears to support engagement, but the relationship is not linear**  
The dashboard shows differences in repeat usage across trust levels, but the pattern does not consistently increase from low trust to very high trust. This suggests that trust score alone may not explain repeat usage. Factors such as verification status, transaction experience, transaction frequency and successful completion may also influence whether users continue using the platform.  
Therefore, trust should be analysed as part of a broader behavioural framework rather than treated as a standalone retention metric.

**9. Verified users form the largest repeat-user group**  
Verified users accounted for **1,797 repeat users**, considerably more than pending **(626)** and unverified users **(576)**.  
This suggests that verification may be associated with stronger continued engagement and could potentially play an important role in building confidence within the P2P marketplace.  
However, further analysis would be required to determine whether verification itself drives retention or whether users who are already more engaged are simply more likely to become verified.

**10. The transaction experience, risk and retention problems are connected**  
The three dashboards collectively show that transaction performance, risk and user retention should not be treated as separate problems.  
Poor transaction experiences can create cancellations and disputes. Repeated disputes and failed transactions can reduce user confidence, while poor experiences may eventually affect repeat usage.  
This means improving the platform should involve looking at the complete user journey, from transaction creation and payment through fulfilment, dispute resolution and repeat usage, rather than optimising each metric independently.  

## Recommendations  
**1. Improve the transaction funnel**  
Focus on the stages with the largest drop-offs, particularly the movement from payment confirmation through delivery confirmation and final fund release.  
**Possible actions include:**  
- Automated reminders for incomplete transactions  
- Clearer delivery and confirmation instructions  
- Notifications when transactions remain inactive  
- Monitoring unusually long completion times

**2. Reduce cancellation and payment failures**  
Investigate the major reasons behind cancelled and failed transactions.  
**The platform could monitor:**  
- Payment failure patterns  
- Payment methods with higher failure rates  
- Transaction categories with high cancellation rates  
- User groups with repeated failed transactions

**3. Strengthen dispute prevention**  
The leading dispute reasons should be incorporated into preventive measures.  
**For example:**  
- Improve transaction descriptions  
- Provide clearer buyer/seller expectations  
- Strengthen delivery confirmation processes  
- Monitor repeated dispute patterns  
- Improve communication around payment-related issues

**4. Prioritise high-risk transactions**  
Fraud-risk transactions should be monitored using behavioural and transaction-level signals such as:  
- Transaction frequency  
- Transaction value  
- Cancellation behaviour  
- Previous disputes  
- Verification status  
- Unusual transaction patterns  
Higher-risk transactions can receive additional verification or review before funds are released.  

**5. Investigate major sources of financial loss**  
The countries with the highest lost transaction value should receive deeper investigation to determine whether the losses are driven by:  
- Higher transaction volumes  
- Higher dispute rates  
- Fraud  
- Refunds  
- Transaction values  
- Operational issues

**6. Strengthen user retention**  
Since repeat users form a significant portion of active users, the platform should identify and replicate the behaviours associated with successful repeat usage.  
**Potential areas include:**  
- Improving the first transaction experience  
- Encouraging user verification  
- Reducing transaction friction  
- Improving trust and reputation signals  
- Personalised engagement for inactive users

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

**Created → Payment Attempted → Payment Confirmed → Delivery Marked → Buyer Confirmed → Funds Released**
