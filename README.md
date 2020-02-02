# Car-Brands-Consumer-Perception-Analysis-Edmunds
 ![](https://manofmany.com/wp-content/uploads/2019/05/8-Top-Australian-Car-Brands-to-Rev-You-Up-feature.jpg)
 
This project is a part of the coursework for Text Analytics at the University of Texas at Austin. Here we scrapped Edmunds.com and implemented various text mining concepts to understand the consumer opinion on car brands and derive insights.

## Table of contents
- [Business Problem](https://github.com/anshikaahuja/Car-Brands-Consumer-Perception-Analysis-Edmunds/blob/master/README.md#business-problem)
- [Data Used](https://github.com/anshikaahuja/Car-Brands-Consumer-Perception-Analysis-Edmunds/blob/master/README.md#data-used)
- [Approach](https://github.com/anshikaahuja/Car-Brands-Consumer-Perception-Analysis-Edmunds/blob/master/README.md#approach)
- [Analysis and Insights](https://github.com/anshikaahuja/Car-Brands-Consumer-Perception-Analysis-Edmunds/blob/master/README.md#analysis-and-insights)

## Business Problem
Edmunds.com is an online resource for automative information. People post reviews about various cars and use the wesbite for awareness building and research. As an analytics consultant to a (i) brand manager, (ii) product manager and (iii) advertising manager, our job was to give advice/insights to these individuals based on the analysis of social media conversations on the website

## Data Used
We scraped around 4000-5000 posts about midsize sedans from [Edmunds](https://forums.edmunds.com/discussion/7526/general/x/midsize-sedans-2-0/p%22) using Selenium. The scraped data can be found in `data.csv`

## Approach
In this project the following steps were taken:
1. Write a scraper using Selenium on python to fetch posts from Edmunds.com
2. Identify the top 10 brands being discussed using frequency counts. Here we replaced car model names with their brand names using the mapping file `models.csv`.
3. Calculate lift scores between brands to identify association between the brands . Plot a multi-dimensional scaling (MDS) map to visualize these relationships.
4. Offer some insights to brand managers for brands identified in the above step.
5. Identify the top 5 most frequently mentioned attributes which people associate with the top brands.
6. Provide suggestions to brand managers of the identified brands based on the above step.
7. Identify the most aspirational brand which people actually want to buy or own from the discussions in the post. What are the business implications of this brand?

## Algorithms/Libraries Used
- Scraper using Selenium
- Word Frequency analysis using NLTK
- Lift scores and MDS map to identify associations

## Analysis and Insights

**1. Top 10 brands**

Brand | Frequency
------------ | -------------
honda | 2237
ford | 1409
toyota | 1103
hyundai | 659
mazda | 606
nissan | 601
chevrolet | 316
saturn | 301
chrysler | 266
subaru | 166

**2. MDS Map**

**3. Advise to managers**
   
Brand to Brand Lift values -
The lift values of Chevrolet and Saturn are very high. So probably they are each other's biggest competitors and have very similar      cars in the midsize sedans category. Both these companies can leverage this and being mentioned with the other brand would be helpful    in promoting the brand.

MDS Plot -
What we could find from the analysis is that Asian brands dominate the midsize Sedan market in the US. FORD is the only US brand in      the top 5, which means there are some attributes that stand out for Ford compared to rest of US brands. In the MDS plot above, FORD      seems to have a place of its own, which provides evidence to our findings.

Our recommendation to FORD Management: We are not finding the above trend carried over to the aspiration score. FORD is being talked    about a lot, so it is worth investigating the associated customer sentiments and preferences. With proper marketing and branding of      DISTINCT features, FORD can challenge for the top spot.

**4. Top attributes**

Attribute | Frequency
------------ | -------------
Design | 3899
Engine | 2562
Pricing | 2552
Year | 1283
Models | 1119
Manufacturer | 1032
Rankings/Rating/Reviews | 771
Safety | 355
Efficiency | 159
Pickup | 34

**5. Advise to managers**
  
Brand to Attribute lift -
Mazda and Chevrolet have an exceptionally good lift with pickup, which could also mean that people are mentioning about pickup trucks   of these brands in the discussion about midsize sedans. This could mean people talk about pickup trucks of these brands while talking   about sedans. This is a business opportunity for Mazda and Chevrolet to expand their pickup truck business by associating with sedans. 

**6. Aspirational brand**

As we can observe from the lift ratios between brands and aspirations, Mazda seems to be the most aspirational brand and people are      showing interest in buying Mazda cars in the future. Our advice to the managers would be to prepare for the forecasted demand and        manufacture accordingly. This should lead to higher revenues and profits for Mazda. The product managers of Mazda can also try to        check what attributes of the cars are making people want to buy them and the advertising managers can advertise more on those            attributes to acquire more customers.

On the other hand, brands with low lift scores like Nissan should be concerned since their low lift scores means that people are not    aspiring to own their brands. Product managers can try to introduce new features which may bring a change. Advertising managers can      try to market the important attributes in such a way that it changes people's perceptions towards the brands.
