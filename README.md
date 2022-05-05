# Starbucks offers Analysis using Python

When it comes to Starbucks this topic is a personal favorite of mine just because I cannot start my day without Starbucks coffee. Starbucks is synonymous with drinking coffee, eating muffins, working with a laptop, and looking for solutions for data science online. I spent a lot of time at Starbuck. The content of the work is an analysis of Starbucks customers and offer data in order to give a corresponding recommendation of an offer type.

I combined transaction, demographic, and offer data to determine which demographic groups respond best to which offer type. In this data analysis, I implement the CRISP-DM-based method for this data analysis. CRISP-DM is a process that is widely used in the analytics model. It includes the following phases: Data Understanding, Data Preparation, Modeling, Evaluation, and Deployment.

Once every few days, Starbucks sends out offers to users of the mobile app. An offer can be merely an advertisement for a drink or an actual offer such as a discount or BOGO (buy one get one free). Some users might not receive any offers during certain weeks. Here, I got the data set that contains simulated data that mimics customer behavior on the Starbucks rewards mobile app. Before the data analysis, I would like to provide a basic introduction to the data set. For the rewards from Starbucks, every offer has a validity period before the offer expires.

## Libraries
In addition to importing pandas, numpy, os, matplotlib and multiple sklearn models, all the plots applied in the analysis requires the installation of plotly and cufflinks for interactive plots, and gmaps for mapping.

## Motivation
Starbucks possesses a unique way of connecting with and rewarding its customers who purchase its products. As an example, a BOGO offer might be valid for only 5 days. we'll see in the data set that informational offers have a validity period even though these advertisements are merely providing information about products, for example, if an informational offer has 7 days of validity, you can assume the customer is feeling the influence of the offer for 7 days after receiving the advertisement. However, it is believed that the data set we used in this analysis may provide an effective reference for Starbucks to identify the function of rewards offers.

I combined transaction, demographic, and offer data to determine which demographic groups respond best to which offer type. In this data analysis, I implement the CRISP-DM-based method for this data analysis. CRISP-DM is a process that is widely used in the analytics model. It includes the following phases: Data Understanding, Data Preparation, Modeling, Evaluation, and Deployment.

1.What is the average income for Starbucks customers?
2.What is the average age for Starbucks customers?
3.What is the most common promotion?
4.What are the most common age and gender?
5.Who is the most loyal customer?
6.What is the most common promotion for children, teens, young adults, and elderly customers?
7.which gets more income from males or females?
8.Which type of promotions does each gender likes?

## File Descriptions
1. The datasets that we have and we are going to read, clean, and analyze:

  * **portfolio.json** —explanation of each variable in the file:
    - id: offer id
    - offer_type
    - difficulty: minimum required spend to complete an offer
    - reward: stars given for completing an offer
    - duration: time for offer to be open, in days
    - channels
  * **profile.json** —explanation of each variable in the file:
    - age
    - became_member_on: date when customer created an app account
    - gender
    - id: customer id
    - income
  * **transcript.json** —explanation of each variable in the file:
    - event: record description (transaction, offer received, viewed, etc.)
    - person: customer id
    - time: time in hours since start of an offer
    - value: either an offer id or transaction amount depending on the event

2. **starbucks_analyze_a_coffee.ipynb** 

## Results
My post in Medium shows the main findings of the analysis.
  * [**Starbucks offers Analysis using Python**](https://medium.com/@tanaviprakashborhade/starbucks-offers-analysis-using-python-40d35f57abb2)

A summary of the findings:
1.The mean is 65404.991568296799. It's not that low but put in mind that this is their annual income. The average income user in the middle-income group is 65000–70000.
2. The average Aged user is middle age around 50–62 years.
3. BOGO and Discount seem the most and they are close to each other with BOGO being slightly higher.
4. Most customers of all gender types. Most of the female customers make between 60k and 70k while most male customers make above 80k. So, the most common are Adults and Male.
5. we can see their Profile ID as each customer has a unique number, Number of Completed Offers, and the Amount. With this data, we can give them extra and unique promotions in order to reward in report image.
6. We can observe that all of them have similar results in offer type, Transactions has the upper hand, followed by BOGO. We can also see that young adults and teens aren't our main customer group, so we can focus on the elderly and adults.
7. The income median for females (around 70k) is higher than for males (around 60k) we can also see that for females the income spreads from 40k to 100k. For males, most of them are around 40k to 70k which is close to the median.
8. Male and Female prefer BOGO. In Others(O), BOGO and discounts are the same, but we can't ignore discounts and the difference between them is low.


## Licensing and Acknowledgement
The datasets used in this analysis were provided by Udacity. Also, plotly provides examples of codes for different types of plots of which some have been adapted, edited, and used as needed.
