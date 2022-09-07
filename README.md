# Repository of Land Classification in Satellite Images by Injecting Traditional Features to CNN Models
More information: https://arxiv.org/abs/2207.10368

Deep learning methods have been successfully applied to remote sensing problems for several years. Among these methods, CNN based models have high accuracy in solving the land classification problem using satellite or aerial images. Although these models have high accuracy, this generally comes with large memory size requirements. On the other hand, it is desirable to have small-sized models for applications, such as the ones implemented on unmanned aerial vehicles, with low memory space. Unfortunately, small-sized CNN models do not provide high accuracy as with their large-sized versions. In this study, we propose a novel method to improve the accuracy of CNN models, especially the ones with small size, by injecting traditional features to them. To test the effectiveness of the proposed method, we applied it to the CNN models SqueezeNet, MobileNetV2, ShuffleNetV2, VGG16, and ResNet50V2 having size 0.5 MB to 528 MB. We used the sample mean, gray level co-occurrence matrix features, Hu moments, local binary patterns, histogram of oriented gradients, and color invariants as traditional features for injection. We tested the proposed method on the EuroSAT dataset to perform land classification. Our experimental results show that the proposed method significantly improves the land classification accuracy especially when applied to small-sized CNN models.
Hi, welcome to my research :)

I would like to special thanks to my professeurs and supporters.

Beril Sirmacek b.sirmacek@saxion.nl and Cem Unsalan cem.unsalan@marmara.edu.tr

![EuroSAT Sample Images](https://github.com/mcagriaksoy/EuroSAT-Image-Classification-with-Wide-and-Deep-Learning/blob/main/eurosat_overview.jpg)

# Dataset Preparation 
This will connect to my drive and copy the contents from my related drive path.
The dataset is gathered from Kaggle: https://www.kaggle.com/apollo2506/eurosat-dataset


> This dataset is being used for classifying the use of land in geospatial images. The end goal for the classification is that the top 2 uses of land in an image are given as output to the user.

> This dataset contains images belonging to the EuroSat dataset. It contains RGB images collected from the Sentinel Dataset.


It has 10 classes that represents the field of:

    AnnualCrop
    Forest
    HerbaceousVegatation
    Highway
    Industrial
    Pasture
    PermanentCrop
    Residential
    River
    SeaLake

Each image is 64x64 pixels with a Ground Sampling Distance of 10m. They were all collected from the Sentinel-2 satellite. But we are resized them to 32x32 to less training time requirements.

# Data Gathering
In this step, the data will be gathered and processed (making ready) for the cnn model feeding.
Our dataset has the json file that describes the classes of each image and with this info we classify them on. We also resize whole dataset as 32x32 which is minimum acceptable resolution for many famous models.

will be updated...

2021 - Created By Mehmet Çağrı Aksoy (Software Engineer)
