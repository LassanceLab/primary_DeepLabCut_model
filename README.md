---  
tags:  
  - github-landing  
alias:  
  -   
author: Thorbjörn Sievert  
Created_at: 2023-09-19 13:51  
Modified_at: 2023-10-23 15:27  
owner: LassanceLab  
repo: primary_DeepLabCut_model  
share: true  
path: /  
title: README  
---  
  
# Main DeepLabCut Model Data of the Lassance Lab  
  
## Description  
The Lassance Lab publishes here the progress of their DeepLabCut model.  
Labelled frames and all previous iterations are included, full video files are not.  
  
## Release Versioning  
We will deviate from standard releases patterns for this repository:  
- Major versions: milestones such as publications or similar  
- Minor versions: Model iterations building up to the next publication  
  
## Model Details  
The model uses mainly the standard tracking labels as used in [ModelZoo](https://deeplabcut.github.io/DeepLabCut/docs/ModelZoo.html) `superanimal_topviewmouse`, plus a few additional tracking points tailored to our needs.  
  
Here are the additional labels:  
  
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
  
  
## Acknowledgments  
We would like to thank the Mathis Labs for developing DeepLabCut. Visit them at <https://github.com/DeepLabCut/DeepLabCut>  
