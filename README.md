# DATA245_-Delivery_time_prediction

### Abstract
The pandemic has made the world gear towards a more digital world and greatly
influenced internet shopping habits. According to a Survey, online retail sales increased 40% in
the US in the year 2020. With the growing e-commerce sales and demand, predicting the correct
delivery dates will help gain customer’s trust and thus benefit the retailers. So, the accuracy of
shipping estimates plays a significant role in providing a hassle-free and trusty customer
experience. Despite the importance of the issue, there hasn’t been much research done on this
particular topic in the machine learning world.
This project focused on how to apply Machine Learning to build a model that can
accurately predict delivery dates for items sold by a retailer using a dataset with details of
shipping information. For our analysis, we decided to train and implement multiple machine
learning models, consisting of Linear Regression, Random Forest, Gradient Boosting Model
(GBM), Support Vector Machine (SVM), and a final ensemble model. To score the model, we
will be looking at RMSE (Root-mean-square deviation).
Keywords: Random Forest, GBM, Delivery date, Machine Learning.
### Motivation
Predicting delivery times has long been an aspect of daily logistics, but refining accuracy
has only lately been critical for services. To satisfy its customers, food services must receive an
order and have it delivered within 30 minutes. In these cases, a variation of just 5 minutes can
make a major impact, thus it's critical for customer satisfaction that the initial projection is
spot-on and any delays are clearly conveyed. Estimated Delivery Dates allow your e-commerce
to show and manage the estimated delivery date for a product to your consumer. Predicting
Accurate Delivery dates is a challenging task. When it comes to providing a hassle-free and
reliable client experience, the accuracy of delivery estimates is critical. When a shipment comes
after the estimated delivery date (“late shipment”), it is a worse experience for the buyer than
when it arrives before the estimated delivery date (“early shipment”). Our team opted to conduct
research into forecasting Estimated Delivery Time and is driven to create the best accurate model
possible because it may be applied to a variety of industries.

### Methodology
In this project, we will focus on implementing machine learning algorithms such as
Random Forest, Linear regression, gradient boosting, bagging regression, Adaboost to achieve
the goal of predicting a delivery date for customers. Furthermore, we have formulated different
scenarios related to different models, sizes for training, and test datasets to find the best
performance for the model. We will compare all these algorithms to identify which algorithm is
appropriate for the prediction task.
### Project Design:
![image](https://user-images.githubusercontent.com/60303995/143147739-a723193e-28cb-4af2-8f7d-c5d0f70d3a67.png)

### Evaluation Methods:
An optimal model will never make mistakes in predicting the delivery date for each shipment
placed by a customer. However, since machine learning is inductive and not deductive, it is hard
to achieve 100% accuracy for a model. Thus, for this task, we will create a penalty function
where we will assign different weights for the late shipments compared to early shipments. Here
is the mathematical representation of this function:
𝐿 = 1/𝑁 * [𝑃𝐸 * ∑ 𝑒𝑎𝑟𝑙𝑦 𝑠ℎ𝑖𝑝𝑚𝑒𝑛𝑡𝑠 + 𝑃𝐿 * ∑ 𝑙𝑎𝑡𝑒 𝑠ℎ𝑖𝑝𝑚𝑒𝑛𝑡𝑠 ]
𝑤ℎ𝑒𝑟𝑒 𝑃𝐸 = 0. 6 , 𝑃𝐿 = 0. 4 , 𝑁 = 𝑛𝑢𝑚𝑏𝑒𝑟 𝑜𝑓 𝑟𝑒𝑐𝑜𝑟𝑑 𝑖𝑛 𝑑𝑎𝑡𝑎𝑠𝑒𝑡
Likewise, Early and late shipments are the difference between actual date and the predicted
date for the delivery
