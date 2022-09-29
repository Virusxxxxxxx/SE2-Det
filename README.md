# SE2-Det
This project is the official implementation of this paper:

**Semantic-Edge-Supervised Single-Stage Detector for Oriented Object Detection in Remote Sensing Imagery**[[paper](https://www.mdpi.com/2072-4292/14/15/3637)]

Core code will be coming soon. Stay tuned...

The repo is based on [MMRotate](https://github.com/open-mmlab/mmrotate) which is a powerful framework for object detection in aerial images, which contains a lot of useful algorithms and tools.

## Abstract
<div align="center">
<img alt="pipeline" src="https://github.com/Virusxxxxxxx/SE2-Det/blob/master/resources/pipeline.png?raw=true" width="1000"/>
</div>

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

## Main Results
* Results on DOTA

| Method  | Dataset  | Backbone   | Input Size  | mAP  |
| ------- | -------- | ---------- | ----------- | ---- |
| SE2-Det | HRSC2016 | ResNet-50  | 1024 x 1024 | 76.4 |
| SE2-Det | UCAS-AOD | ResNet-101 |  800 x 800  | 90.0 |

* Visualization results on the test set of DOTA.

<img src="https://github.com/Virusxxxxxxx/SE2-Det/blob/master/resources/dota.png?raw=true" width="1000"/>

* Visualization results on UCAS-AOD.

<img src="https://github.com/Virusxxxxxxx/SE2-Det/blob/master/resources/ucas.png?raw=true" width="1000"/>

# Citation

If you find our work or code useful in your research, please consider citing:

```
@Article{rs14153637,
AUTHOR = {Cao, Dujuan and Zhu, Changming and Hu, Xinxin and Zhou, Rigui},
TITLE = {Semantic-Edge-Supervised Single-Stage Detector for Oriented Object Detection in Remote Sensing Imagery},
JOURNAL = {Remote Sensing},
VOLUME = {14},
YEAR = {2022},
NUMBER = {15},
ARTICLE-NUMBER = {3637},
URL = {https://www.mdpi.com/2072-4292/14/15/3637},
ISSN = {2072-4292},
DOI = {10.3390/rs14153637}
}
```
