## Overview
This repository explores data collected with the intent to inform a digital mobile coupon distribution strategy.

The dataset includes user, contextual, and coupon attributes:

User attributes:
- Gender
- Age
- Marital Status
- Number of children
- Education, Occupation
- Annual income
- Number of times that he/she goes to a bar
- Number of times that he/she buys takeaway food
- Number of times that he/she goes to a coffee house
- Number of times that he/she eats at a restaurant with average expense less than $20 per person

Contextual attributes:
- Driving destination
- Location of user, coupon and destination
- Weather
- Temperature
- Time
- Passenger

Coupon attributes:
- time before it expires: 2 hours or one day

## Findings

### Findings regarding Coffee House Coupons:
Overall, the odds of a user accepting a coffee house coupons was very close to 50/50.

However, exploratory data analysis reveals some situations where coffee House coupons have notably higher rates of acceptance:
- when it is late morning or early afternoon in the day (59%)
- when a user is not alone and not with kids (59%)
- when the user is on a leisure trip rather than driving to work or home (58%)
- when the user is known to frequent coffee houses (67%)
- by students and unemployed individuals (57%)
- when the expiration is a day rather than 2 hours (58%)

### Visualization of these relationships:
![Coupon Acceptance for time](./plots/Coupon%20Acceptance%20Count%20by%20time.png)
![Coupon Acceptance for passenger](./plots/Coupon%20Acceptance%20Count%20by%20passenger.png)
![Coupon Acceptance for destination](./plots/Coupon%20Acceptance%20Count%20by%20destination.png)
![Coupon Acceptance for Coffee House](./plots/Coupon%20Acceptance%20Count%20by%20CoffeeHouse.png)
![Coupon Acceptance for occupation](./plots/Coupon%20Acceptance%20Count%20by%20occupation.png)
![Coupon Acceptance for expiration](./plots/Coupon%20Acceptance%20Count%20by%20expiration.png)

## Recommendations
With respect to the coffee house coupons, not all determinants are knowable at the time of issuance of coupons. For example, we can know the time of day; we may not know if a recipient has child with them.

An ROI analysis should be performed on sending coupons based on knowable determinants. Though it may be possible that it is profitable to send coupons regardless of determinants, it is likely that now, or in the future it will be cost effective only above a certain threshold of acceptance. The greatest acceptance would be expected with the conditions listed above. Further analysis could seek to identify other higher acceptance subpopulations by further exploring combinations of determinants.

> [ View Analysis Details ](./analysis.ipynb)&nbsp;<img src="./images/j-notebook.png" alt="jupyter notebook" style="width:14px;"/>
