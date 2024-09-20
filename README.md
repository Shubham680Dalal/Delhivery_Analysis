# Non-Efficient Trips Analysis

## Overview
This analysis is based on training data post-missing value and outlier treatment. The insights assume **no waiting time per stop** during trips.

## Problem Statement
The objective of this analysis is to evaluate the impact of the current OSRM (Open Source Routing Machine) and provide insights on non-efficient trips. This evaluation primarily focuses on trips with inefficiencies in the estimated versus actual travel times.



### Key Observations
Non-Efficient trips are common in specific regions, particularly from **North and East India**, and are prevalent in trips passing through hilly, forested, or underdeveloped roads. These trips often involve frequent stops, and the estimated times provided by OSRM are significantly lower than the actual travel times.

### Examples of Non-Efficient Routes:
- Himachal Pradesh to Punjab
- Jammu & Kashmir to Punjab
- Meghalaya to Assam
- Nagaland to Assam
- Assam to Tripura
- Telangana to Andhra Pradesh

For these routes, **actual trip times are approximately double** the estimated OSRM times.

### Triggered Time Periods:
**Evening trips**, which are assumed to be the most trafficked part of the day, are the least efficient. These trips average **6 stops per route** and experience significant discrepancies between estimated and actual travel times. 

The current OSRM estimates are overly optimistic, providing time estimates that are roughly **half the actual time**. These estimates do not adequately account for traffic conditions, which are especially problematic during peak traffic hours.

## Optimization Strategies

### Route Optimization
- **Strategic stop planning**: By reducing the number of stops and selecting less congested routes or better roads, particularly on **Non-Efficient Trip Routes**, significant time savings can be achieved.
- **Evening trips**: Reducing the number of service or transit stops during **evening trips**, when traffic is heaviest, can lead to marked improvements in route efficiency.

### OSRM Version Improvements
To improve the accuracy of route estimations, it is recommended to use an **OSRM version** that factors in stops along the route. This will help provide more accurate travel time estimates, especially on trips with frequent stops. An **OSRM estimation algorithm** that accurately reflects Indian traffic, road conditions, and frequent stops is essential for improving trip efficiency.





