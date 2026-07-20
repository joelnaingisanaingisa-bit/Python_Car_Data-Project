### Fleet Fuel Efficiency Advisory Analysis
Python | Pandas | Matplotlib | Data Analytics Portfolio Project
## Business Problem
# Client scenario:
Nairobi AutoFleet Advisors is a fictional vehicle-
consulting

firm that helps Kenyan businesses — logistics companies, ride-
hailing operators,

and SMEs with company cars — choose vehicles that minimize fuel
spend without
sacrificing capability. With fuel prices rising, a logistics client has
asked
for a data-driven recommendation on which of 32 candidate vehicle
models to
add to their fleet.
# Dataset:
car_fuel_efficiency_32.csv — 32 vehicles with mpg ,
cylinders ,
horsepower , and weight .
# Goal:
Answer 5 business questions to produce a segmented,
evidence-based
purchase recommendation.

## Business Questions & Findings
# Q1 — Which vehicles deliver the best fuel efficiency
overall?

The Kia Rio (37 mpg), Ford Fiesta (36 mpg), and Toyota Corolla (35
mpg) lead
the field. The Chevrolet Equinox and Honda Pilot trail at 22 mpg — a
68%
efficiency gap between the best and worst performer.
https://drive.google.com/file/d/1ZJHuBMg0CRf7g2Bk3KQFcDyEQ-ILvHkc/view?usp=drive_link
# Q2 — How does engine size (cylinders) affect fuel
efficiency?
4-cylinder vehicles average 28.9 mpg versus 24.3 mpg for 6-
cylinder
vehicles. Engine size alone is a meaningful but incomplete signal —
some
4-cylinder SUVs still perform worse than the 6-cylinder average.
https://drive.google.com/file/d/1KX432t3VssstQfcju-hFag3jeu7IJDJP/view?usp=drive_link
# Q3 — Is there a fuel-economy trade-off for horsepower?
Yes: horsepower and mpg correlate at r = -0.75. Every additional
unit of
power comes at a measurable fuel-economy cost, confirming the
classic
performance-vs-efficiency trade-off.
https://drive.google.com/file/d/1cwOR7OIEosTQINPArKQnb0P9OnRqGuHd/view?usp=drive_link
# Q4 — Does vehicle weight predict fuel efficiency?
This is the strongest relationship in the dataset: r = -0.93. Weight is
a
better predictor of fuel economy than horsepower or engine size —
heavier
vehicles are consistently and predictably less efficient.
https://drive.google.com/file/d/1LKbXR39MJ8ZdXnb24448liI2KwJLd7Jm/view?usp=drive_link

# Q5 — Which vehicles should we recommend to each client type?
Vehicles were segmented into three classes to match client use
https://drive.google.com/file/d/1jp91ewQydwByRIs_uaVmSH0MjUJz0f-x/view?usp=drive_link
cases:

Segment

Avg
MPG
Avg
HP
Avg
Weight
Best Pick

Economy
Compact

32.8 99.6
2,507
lbs
Kia Rio (37
mpg)

Midsize
Sedan

26.5 176.8
3,382
lbs
Hyundai
Sonata (31
mpg)

SUV /
Performance

25.0 260.8
3,862
lbs
Subaru
Legacy (27
mpg)

## 📊 q5_segment_recommendation.png

## Recommendation to the Client
For a cost-conscious delivery fleet, the Economy Compact
segment (Kia
Rio, Ford Fiesta, Toyota Corolla) offers the lowest fuel cost per mile
and
should be the default fleet vehicle. For executive or client-facing
roles
where cabin space matters, the Hyundai Sonata is the most
efficient Midsize
option without stepping into SUV-level fuel costs. SUVs should be
reserved
only for use cases that genuinely require the added capability, since

they
carry the highest fuel cost per mile in this dataset.

## Tools & Methods
Python 3, pandas (data wrangling, grouping, correlation)
matplotlib (custom navy/gold branded visualizations)
Feature engineering: rule-based vehicle segmentation
Statistical methods: Pearson correlation, group aggregation,
boxplot distribution analysis
