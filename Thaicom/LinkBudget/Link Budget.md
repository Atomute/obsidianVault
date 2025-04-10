___
Link budget calculation is
## Flow
____
#### Use case 1: Calculate Up
Get G/T and use it to calculate up side.
1. Get G/T (DONE)
2. Calculate (DONE)
	1. Find formula
	2. implement formula 
	3. done
#### Use case 2: Calculate down
Get EIRP from csv and use it to calculate Down side.
1. Get EIRP (DONE)
	1. Problem
		1. Sometime the lat long of the address is not in the datasource. This will get no match.
		2. 
	2. Improve performance. 
		1. Provided data about location address and lat-long. [[LAT-LONG csv]]
		2. Use python to verify the shortest distance lat-long that is fall on the same district.
2. Calculate (DONE)
	1. Find formula
	2. implement formula 
	3. done
#### Next Step
- prepare for more parameter
- Table
	- vary antenna size
- Map


## Note
- Do I need to study link budget calc?
	- to get the idea of it
	- to know the way user ask a question
	- 