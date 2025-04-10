[[Conclusion]]
### Weight
I try adding weight 
## Problem
- Labeler
	- They didn't label based on the actual image (They use google map, which sometime it's not the same time as the train image)
	- The image itself is ambiguous, hard to tell even with the human eye.
	- They randomly pick feature to test
		- I don't know how they pick
		- some feature that's really big always not the selected one like ![[Xaythany_road_one _feature.png]]
		- a big feature like this have to separate into multiple small one.
	
## Notes
- Model assessment is a process that input new dataset to trained model and see how it's doing
	- So you should have labeled dataset for this job
	- You must be certain with your label so that the output will be precise
- class
	- 1 - building
	- 2 - road
	- 3 - null
	- 4 - forest
	- 5 - other
	- 6 - water
	- 7 - grass
## Class with low F1 score
[[Class]]
### Model 012b_bolihhamxay
[[Model 012b_bolihhamxay]] 
- Road (0.020)
	- f1-score: 0.020 precision: 0.011 recall: 0.214 support: 14
- Other (0.345)
	- f1-score: 0.345 precision: 0.421 recall: 0.293 support: 536
### Model 012b_vientiane
- Road
	- f1-score: 0.257 precision: 0.150 recall: 0.900 support: 50
- Other
	- f1-score: 0.429 precision: 0.650 recall: 0.320 support: 766
### Model 012b_xaythany
- Road
	- f1-score: 0.135 precision: 0.074 recall: 0.733 support: 30
- Forest
	- f1-score: 0.204 precision: 0.128 recall: 0.500 support: 74
- Other 
	- f1-score: 0.350 precision: 0.529 recall: 0.262 support: 729
### Model 012c_bkc
- Road
	- f1-score: 0.094 precision: 0.074 recall: 0.132 support: 38
- Forest
	- f1-score: 0.198 precision: 0.131 recall: 0.407 support: 27
- Other
	- f1-score: 0.137 precision: 0.096 recall: 0.239 support: 71
### Model 012c_cnx
- Forest
	- f1-score: 0.169 precision: 0.095 recall: 0.750 support: 8
- Other
	- f1-score: 0.385 precision: 0.282 recall: 0.603 support: 58
### Model 012c_eec
- Road
	- f1-score: 0.184 precision: 0.105 recall: 0.731 support: 26
- Forest
	- f1-score: 0.134 precision: 0.081 recall: 0.378 support: 37
- Other
	- f1-score: 0.481 precision: 0.507 recall: 0.457 support: 372
### Model 021x_bkc
- Road
	- f1-score: 0.298 precision: 0.875 recall: 0.179 support: 39
- Forest
	- f1-score: 0.082 precision: 0.044 recall: 0.600 support: 10
- Other
	- f1-score: 0.055 precision: 0.034 recall: 0.138 support: 29
### Model 021x_cnx
- Water
	- f1-score: 0.455 precision: 0.714 recall: 0.333 support: 30
- Other
	- f1-score: 0.296 precision: 0.327 recall: 0.271 support: 133
### Model 021x_eec
- Road
	- f1-score: 0.279 precision: 0.227 recall: 0.362 support: 141
- Other
	- f1-score: 0.329 precision: 0.383 recall: 0.288 support: 479