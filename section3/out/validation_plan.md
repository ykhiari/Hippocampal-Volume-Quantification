## What is the intended use of the product?  
This algorithm is intended to be used as an assistance for radiologists in identifying hippocampus volumes.


## How was the training data collected?  
We are using the "Hippocampus" dataset from the Medical Decathlon competition. This dataset is stored as a collection of NIFTI files, with one file per volume, and one file per corresponding segmentation mask. The original images here are T2 MRI scans of the full brain. As noted, in this dataset we are using cropped volumes where only the region around the hippocampus has been cut out. This makes the size of our dataset quite a bit smaller, our machine learning problem a bit simpler and allows us to have reasonable training times.
The dataset can be found in http://medicaldecathlon.com/. The dataset consists of 263 training and 131 testing images.  

## How did you label your training data?  
All data has been labeled and verified by an expert human rater, and with the best effort to mimic the accuracy required for clinical use. To cite this data, please refer to https://arxiv.org/abs/1902.09063

## How was the training performance of the algorithm measured and how is the real-world performance going to be estimated?  
For this specific algorithm the performance was measured by using the following methods:
- Jacard distance
- Dice score

In a real world the performance will be measured by a radioligist.  

## What data will the algorithm perform well in the real world and what data it might not perform well on?
As per the results provided in the result file, the algorithm should perform fairly well in all MRI scan of the brain.
The algorithm has no distinguish weaknesses.

