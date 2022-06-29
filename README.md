# Human Action Recognition using BlazePose Skeleton on Spatial Temporal Graph Convolutional Networks

This is the project repository for the research study *Human Action Recognition using BlazePose Skeleton on Spatial Temporal Graph Convolutional Networks* presented by Motasem S. Alsawadi and Miguel Rio.
*Pending for publication


## Contents
* [1. Download UCF-101 BlazePose skeleton dataset](https://github.com/malswadi/blazepose-skeleton-hmdb-ucf#1-download-ucf-101-skeleton-dataset)
* [2. Download HMDB BlazePose skeleton dataset](https://github.com/malswadi/blazepose-skeleton-hmdb-ucf#2-download-hmdb-skeleton-dataset)
* [3. Storage info](https://github.com/malswadi/skeleton_ucf_hmdb#3-storage-info)
* [Citation](https://github.com/malswadi/skeleton_ucf_hmdb#citation)
* [Acknowledgements](https://github.com/malswadi/skeleton_ucf_hmdb#acknowledgements)

## 1. Download UCF-101 skeleton dataset

The [UCF-101](https://www.crcv.ucf.edu/data/UCF101.php) dataset provides a total of 13,320 clips classified into 101 action classes. The skeleton output layout has been extracted using the [OpenPose](https://github.com/CMU-Perceptual-Computing-Lab/openpose) system. Due to the variability of the duration of each clip, a fixed duration of 300 frames has been proposed. Therefore, if any video clip has less than 300 frames, we repeat the initial frames until reach the amount needed. Otherwise, if the video clip exceeds the frame number, we randomly eliminated the difference in frames. Consequently, the spatio-temporal information of the skeleton of each video sample can be represented as a tensor with shape (33, 3, 300).  An independent JSON file has been exported for each video sample. Thus, the outcome of this process are 13,320 JSON files with the BlazePose skeleton information of the UCF-101 dataset. respectively. The UCF-101 Blazepose skeleton dataset can be downloaded [here](link_to_download).

## 2. Download HMDB-51 skeleton dataset

The [HMDB-51](https://serre-lab.clps.brown.edu/resource/hmdb-a-large-human-motion-database/) dataset provides a total of 6,766 video clips of 51 different classes. Similar to the [UCF-101 skeleton dataset]( https://github.com/malswadi/blazepose-skeleton-hmdb-ucf#1-download-ucf-101-skeleton-dataset), the skeleton output layout has been extracted using the [OpenPose](https://github.com/CMU-Perceptual-Computing-Lab/openpose) system using the same fixed  length of 300 frames. Also, an independent JSON file has been exported for each video sample. Therefore, 6,766 JSON files with the BlazePose skeleton information of the HMDB-51 dataset. The HMDB-51 skeleton dataset can be downloaded [here](link_to_download).

## 3. Storage info
The UCF-101 and HMDB-51 skeleton dataset are provided as .zip format. 

#### UCF-101
Pending

#### HMDB-51
Pending.

## Acknowledgements
The training code is written by Motasem S. Alsawadi and it is based upon the skeleton extraction guidelines provided  in *Spatial Temporal Graph Convolutional Networks for Skeleton-Based Action Recognition*, Sijie Yan, Yuanjun Xiong and Dahua Lin, AAAI 2018. [[Arxiv Preprint]](https://arxiv.org/abs/1801.07455)
