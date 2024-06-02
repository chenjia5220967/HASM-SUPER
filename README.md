# Adaptive Multi-tasks Autoencoder-based Hyperspectral Unmixing Exploiting Auxiliary Data via Graph Networks
#
This article This article is currently being submitted.

or, If you have any question, please do not hesitate to contact me.

chen_jia@cug.edu.cn

Usage
---------------------
## Abstract

Hyperspectral unmixing is a technique in hyperspectral image processing that decomposes the spectra of mixed pixels into pure spectral components (endmembers) and their corresponding contributions (abundances). When dealing with complex mixed terrain scenes, such as in urban areas, significant challenges arise. To address these challenges, this work exploits urban auxiliary information within the framework of an adaptive multi-task autoencoder (AE) unmixing model, utilizing graph networks.
The framework enhances the information in hyperspectral images by utilizing urban auxiliary data. Specifically, it performs superpixel segmentation to subdivide complex urban environments into simpler units. Subsequently, different AE-based unmixing methods are applied to these segmented results. Graph networks are employed to identify similar blocks within the image, incorporating this additional information into the unmixing process.
In the experiments conducted for this work, two hyperspectral unmixing datasets were prepared, along with their corresponding urban auxiliary data. The results demonstrate that the proposed method achieves robust performance, even in the case of complex urban environments.


### tangxun Lake.
<p align="center">
<img src="./structure.png" alt="drawing" width="700"/>

## Preliminary preparation

Torch

Numpy


## Input

image Y



## Output
endmembers and abundances of three different unmixing methods. (saved as a MAT file)



## Testing
    
After training the MAHUM on the datasets, the extracted abundance and endmember results are saved as a MAT file. You can utilize `./displayresult.m` to evaluate the unmixing performance.




## Dataset

Thomson Lake: an airborne hyperspectral image about an area inside the city of Wuhan, China. The hyperspectral dataset consists of $133$ bands with $100*100$ pixels and cover nearly $9km^2$ with the spatial resolution $30m$. The area is characterized by a rather sparse urbanization, with small and narrow roads and buildings that are not very prominent. 

 Pavia: an hyperspectral image of the city of Pavia, Italy,  acquired by the Italian Space Agency (ASI) using the PRISMA satellite. The dataset consists of $199$ bands with $120*120$ pixels and covers nearly $13km^2$ with the spatial resolution $30m$. This dataset is characterized by the fact that the river and channels are difficult to extract at the rather coarse spatial resolution of the spaceborne sensor. In addition, the area has a dense urbanization, with roads and buildings that are intertwined, a situation which makes it difficult to accurately extract a built-up map. 


<p align="center">
<img src="./second.png" alt="drawing" width="400"/>



## Experimental result

### tangxun Lake.
<p align="center">
<img src="./tangxunhu.png" alt="drawing" width="700"/>


### Pavia.
<p align="center">
<img src="./pavia.png" alt="drawing" width="700"/>
