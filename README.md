How can customer preferences and behaviors be leveraged to inform the development of new products,
services, or coupon offerings that align with customer needs? To design and implement machine learning
algorithms capable of predicting whether a customer will accept a coupon from a nearby coffee shop or
restaurant considering the demographic and contextual attributes. Answer that the user will drive there
‘right away’ or ‘later before the coupon expires’ are labeled as Y=1 and answer ‘no, I don’t want the
coupon’ is answered by Y=0. Five types of coupons were investigated: Bars, takeaway food restaurants,
coffee house, cheap restaurant, expensive restaurant. This involves analyzing various driving scenarios
described in the dataset, including details such as destination, weather conditions, passengers, and more, to
discern patterns and make informed predictions about customer decisions regarding coupon acceptance.
This problem can be solved using binary class classification. Some of the rules are: if a customer (goes to
coffee houses ≥ once per month AND destination = no urgent place AND passenger! = kids) OR (goes to
coffee houses ≥ once per month AND the time until coupon expires = one day) Then (predict the customer
will accept the coupon for a coffee house).
DATA RESOURCES: The data for the analysis is taken from UC Irvine’s Machine Learning Repository
https://archive.ics.uci.edu/dataset/603/in+vehicle+coupon+recommendation


There are 12684 rows and 26 features. (Including target variable ‘Y’)
Sr. No. Feature Name Data Type Description of Variable Percentage of
Missing Value
1 Destination String Intended place to visit
(e.g., "No Urgent Place"
or "Home")
-
2 Passenger String Type of passenger (e.g.,
"Alone," "Friend(s),"
"Kid(s)")
-
3 Weather String Weather conditions
during the trip (e.g.,
"Sunny")
-
4 Temperature String Temperature in degrees
during the trip
-
5 Time String Time of the day when
the trip took place (e.g.,
"2PM," "6PM,"
"10AM")
-
6 Coupon String Type of coupon and its
expiration time
(e.g.,"Restaurant(<$20)"
)
-
7 Gender String Gender of the passenger
(e.g., "Female")
-
8 Age String Age of the passenger -
9 Marital Status String Marital status of the
passenger (e.g.,
"Unmarried partner")
-
10 Has children Numeric Indicates whether the person has children (1
for Yes, 0 for No)
-
11 Education String Level of education (e.g.,
"Some college
- no
degree")
-
12 Occupation String Occupation of the person
-
13 Income String Income range of the person
-
14 Car String Whether the person
owns a car (e.g., "never"
or "ever")
99%
15 Bar Numeric Frequency of visits to
bars every month (e.g.,
“never”,”less1”
0.84%
16 CoffeeHouse Numeric Frequency of visits to
Coffee houses every
month (e.g.,
“never”,”less1”)
1.71%
17 CarryAway String Frequency of
t
a
k
e
-away
food every month (e.g.,
“never”, ”less1”)
1.19%
18 RestaurantLessThan20 String Frequency of visits to a
restaurant with an
average expense per
person is less than $20
every month (e.g.,
“never”, ”less1”)
1.02%
19 Restaurant20To50 Numeric Frequency of visits to a
restaurant with an
average expense per
person is between $20
and $50 every month
(e.g., “never”, ”less1”)
1.49%
20 toCoupon_GEQ5min Numeric Driving distance to the
restaurant or bar (1 for
greater than or equal to 5
minutes, 0 for less)
-
21 toCoupon_GEQ15min Numeric Driving distance to the
restaurant or bar (1 for
greater than or equal to
15 minutes, 0 for less)
-
22 toCoupon_GEQ25min Numeric Driving distance to the
restaurant or bar (1 for
greater than or equal to
25 minutes, 0 for less)
-
23. Expiration String Duration to expire (e.g.,
“1d”, “2h”)
24. direction_same String Whether the coupon
place in the same
-
direction in the same
direction as the person’s
current destination? (1
for yes and 0 for no)
25 direction_opp String Whether the coupon
place in the opposite
direction in the same
direction as the person’s
current destination? (1
for yes and 0 for no)
-
26 Y Numeric The target variable
indicating whether the
passenger used a coupon
(1 for Yes, 0 for No) 
