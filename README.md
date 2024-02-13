---  
tags:  
  - github-landing  
alias: []  
author: Thorbjörn Sievert  
Created_at: 2023-09-19 13:51  
Modified_at: 2024-01-08 14:57  
owner: LassanceLab  
repo: primary_DeepLabCut_model  
share: true  
path: /  
title: README  
---  
  
# Main DeepLabCut Model Data of the Lassance Lab  
  
## Description  
The Lassance Lab publishes here the progress of their DeepLabCut model.  
Labeled frames and all previous iterations are included, full video files are not.  
  
## Release Versioning  
We will deviate from standard release patterns for this repository:  
- Major versions: milestones such as publications or similar  
- Minor versions: Model iterations building up to the next publication  
  
## Model Details  
  
The current model contains the following data:  
  
Frames (n):  
  
| Strain | Female | Male | Total |  
|:------:|:------:|:----:|:-----:|  
|   BW   |   560   | 495  |  1055  |  
|   PO   |  530   |  570  |  1100  |  
| Total  |  1090   | 1065  |  2155  |  
  
Animals (n):  
  
| Strain | Female | Male | Total |  
|:------:|:------:|:----:|:-----:|  
|   BW   |   15    |  14   |   29   |  
|   PO   |   15    |  16   |   31   |  
| Total  |   30    |  30   |   60   |  
  
### Animals  
We currently use *Peromyscus polionotus* (PO) and *Peromyscus maniculatus* (BW) of both sexes in our model.  
  
### Camera and Setup  
Videos are recorded at 1440 x 1080 pixels, 200fps. All videos are recorded in black and white, under red light conditions.  
We are currently using two Basler acA1440-220μm.  
  
### Keypoints  
The model uses mainly the standard tracking labels as used in [ModelZoo](https://deeplabcut.github.io/DeepLabCut/docs/ModelZoo.html) `superanimal_topviewmouse`, plus a few additional tracking points tailored to our needs.  
  
Here are the additional keypoints:  
  
```yaml  
- chin #for rearing animals to properly track head movement  
  
- throat #same as above  
  
- tl_corner #top left corner to draw cage layout in R   
  
- tr_corner #top right   
  
- bl_corner #bottom left  
  
- br_corner #bottom right   
  
- petri_12 #12 o'clock position of the petri dish. Indicated with 3 dots on the rim   
  
- petri_03 # 3 o'clock position of the petri dish. Relative to the previous 12 o'clock position   
  
- petri_06  
  
- petri_09  
  
- petri_12_3 # Halfway between the 12 o'clock and 3 o'clock position  
  
- petri_3_6  
  
- petri_6_9  
  
- petri_9_12  
```  
  
  
<details>  
<summary><h2>Version Overview</h2></summary>  
  
### 0.5  
  
Iteration 5 of our model  
  
Frames (n):  
  
| Strain | Female | Male | Total |  
|:------:|:------:|:----:|:-----:|  
|   BW   |   560   | 495  |  1055  |  
|   PO   |  530   |  570  |  1100  |  
| Total  |  1090   | 1065  |  2155  |  
  
Animals (n):  
  
| Strain | Female | Male | Total |  
|:------:|:------:|:----:|:-----:|  
|   BW   |   15    |  14   |   29   |  
|   PO   |   15    |  16   |   31   |  
| Total  |   30    |  30   |   60   |  
  
### 0.3 Initial Release  
  
Iteration 3 of our model.  
  
Frames (n):  
  
| Strain | Female | Male | Total |  
|:------:|:------:|:----:|:-----:|  
|   BW   |   80   | 120  |  200  |  
|   PO   |  100   |  40  |  140  |  
| Total  |  180   | 160  |  340  |  
  
Animals (n):  
  
| Strain | Female | Male | Total |  
|:------:|:------:|:----:|:-----:|  
|   BW   |   2    |  2   |   4   |  
|   PO   |   3    |  1   |   4   |  
| Total  |   5    |  3   |   8   |  
  
</details>  
  
## Acknowledgments  
We would like to thank the Mathis Labs for developing DeepLabCut. Visit them at https://github.com/DeepLabCut/DeepLab