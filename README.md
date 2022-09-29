# Semantic-Edge-Supervised Single-Stage Detector for Oriented Object Detection in Remote Sensing Imagery

![](demo/overall_pipeline.png)

The repo is based on [MMRotate](https://github.com/open-mmlab/mmrotate) which is a powerful framework for object detection in aerial images, which contains a lot of useful algorithms and tools.

## Abstract
In recent years, significant progress has been made in arbitrary-oriented object detection.
Different from natural images, object detection in aerial images remains its problems and challenges.
Current feature enhancement strategies in this field mainly focus on enhancing the local critical
response of the target while ignoring the target’s contextual information, which is indispensable for
detecting remote sensing targets in complex backgrounds. In this paper, we innovatively combine
semantic edge detection with arbitrary-oriented object detection and propose a feature enhancement
network base on a semantic edge supervision module (SES) that realizes an attention-like mechanism
in three dimensions of space, channel, and pyramid level. It helps the network pay attention to
the edge features of targets at multiple scales to obtain more regression clues. Furthermore, to
solve the problem of dense objects with different directions in remote sensing images, we propose a
rotation-invariant spatial pooling pyramid (RISPP) to extract the features of objects from multiple
orientations. Combining the two feature enhancement modules, we named the network SE 2 -Det,
extensive experiments on large public datasets of aerial images (DOTA and UCAS-AOD) validate
our approach’s effectiveness and demonstrate our detector’s superior performance.

## Results
