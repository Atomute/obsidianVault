### Problem
- They didn't label based on the actual image (They use google map, which sometime it's not the same time as the train image)
- The image itself is ambiguous, hard to tell even with the human eye.
- They randomly pick feature to test
	- I don't know how they pick
	- some feature that's really big always not the selected one like ![[Xaythany_road_one _feature.png]]
	-  a big feature like this have to separate into multiple small one.
### Forest and Grass
- did not merge forest and grass
- have ambiguous definition for class grass, forest and other
- ambiguous image

## Other
- the image is hard to tell
- have ambiguous definition for class grass and other
- id
	- 164

## Road
- the main road is one big feature


### Solution
- improve assesment
	- use NDVI, NDWI and some other indicator to help with labeling
	- Skip feature that is not clear as it affect the assessment (Not sure if you can do this)
	- use a high resolution image of the area at the same time to help labeling
- improve model
	- Split big feature to multiple small features (especially road, forest, grassland)
	- don't predict a very small area (set confidence threshold? or something)