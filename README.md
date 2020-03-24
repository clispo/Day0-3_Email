# Day0-3_Email-v1
Problem Statement:

   Currently, we are sending Day 0 & Day 3 emails to every 7DFT user by default. From previous analysis, we know some people will go directly cancel their account after opening the email, hence causing a higher cancel rate. In this study, we build a Random Forest Classification model on Email openers to determine who should receive Day 0 / Day 3 emails.

Since the impact of Day 0 Email is greater than Day 3 email, and input features are very similar. We will use Day 0 Email as an example.

Input Data: 

'2019-07-17' ~ '2020-01-16' Day 0 Day 3 Email Opens:

Features: 

Device,
Channel,
Card Type,
User's initial conversion state,
Email Domain,
Sign-up Intent,
Operating System,
Purchased Product,
Purchased Product QUality,
First 1-hour Profile Quota View

Response Variable:

A user canceled within 60 minutes after opening the email - 1; Rest - 0.

Overall Performance:

With upsampling, accuracy and recall is around 0.87. 
'Profile Quota View', 'Operation System', 'State', 'Card Type' and 'Purchaseed Product Quality' are important featurees. 

Use Case:

We can use those freatures for next round of A/B testing, if the conclusion stays same, we can keep improving the model, and wrap up the script to production for automation purpose.

