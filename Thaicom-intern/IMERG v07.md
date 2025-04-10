The GPM_3IMERGHHL dataset has undergone updates between versions 6 (V06) and 7 (V07).
- v7 precipitation differ a bit from v6
- will absolutely affect dry spell model, especially in the decision step.
- may have to retrain the model using v7 dataset
![[PDF_6vs7.png]]
[IMERG 7 Release Note](https://gpm.nasa.gov/resources/documents/imerg-v07-release-notes) 
[IMERG 7 vs IMERG 6](https://www.mdpi.com/2072-4292/15/23/5622)
## Code Change
- download_imerg_config.yaml
    - imerg_url 
        - (change 6 to 7)
- preprocess_config.yaml
    - imerg/column/value 
        - precipitation
    - imerg_multiband/column/value 
        - precipitation
        - Intermediate/precipitationUncal
- inference_config.yaml
    - imerg_column
        - precipitation
## Issues
---
1. ValueError: numpy.dtype size changed, may indicate binary incompatibility. Expected 96 from C header, got 88 from PyObject
	*Solved* use the old image as base image
2. Cannot download instantly .
	does'nt seem to be a problem since the original is the same.
3. 