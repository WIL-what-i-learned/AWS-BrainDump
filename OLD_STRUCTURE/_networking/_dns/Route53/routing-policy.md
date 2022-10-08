# Routing Policy

> additional load balancing through RT53

- Simple 👉 used to redirect to a single resource
- Weighted (Canary Deployments)
	- test 1% of traffic on new website
	- split traffic between two reagions
	- can be associated with Health Checks
- Latency Based
	- evaluated in terms of user to designated AWS Region
- Failover
- GeoLocation 👉 based on user location
- GeoProximity
	- set bias
	- shifting traffic from one region to another
- Multi Value Routing