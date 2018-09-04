Title: Revisiting RCNN: On Awakening the Classification Power of Faster RCNN
Slug: revisiting-faster-rcnn
Date: 2018-08-31 19:59:53
Tags: Faster RCNN, Object Detection, 2018, PAPER
Author: Quang Nguyen
Category: paper
TopPost: no

# Abstract 

Recent region-based object detectors are usually built with separate classification and localization branches on top of shared feature extraction networks. In this paper, we analyze **failure cases** of **state-of- the-art detectors** and observe that **most hard false positives** result from **classification** instead of localization. 

We conjecture that:  

1. **Shared feature representation** is not optimal due to the mismatched goals of feature learning for classification and localization; 

2. **Multi-task learning** helps, yet optimization of the multi-task loss may result in sub-optimal for individual tasks; 

3. **Large receptive field** for different scales leads to redundant context information for small objects. We demonstrate the potential of detector classification power by a simple, effective, and widely-applicable Decoupled Classification Refinement (DCR) network. 

DCR **samples hard false positives** from the base classifier in Faster RCNN and trains a RCNN-styled strong classifier. Experiments show new state-of-the-art results on PASCAL VOC and COCO without any bells and whistles.


# More Discussions

DCR demonstrates extremely good performance in suppressing false positives.