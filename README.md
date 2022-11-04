# 3D-CNN-BERT-COVID19: The 4th-place solution for the ICCV-2021 MIA COV19D Competition. 
Implementation of "A 3D CNN Network with BERT For Automatic COVID-19 Diagnosis From CT-Scan Images"
For details, refer to our paper https://arxiv.org/abs/2106.14403 and https://openaccess.thecvf.com/content/ICCV2021W/MIA-COV19D/html/Tan_A_3D_CNN_Network_With_BERT_for_Automatic_COVID-19_Diagnosis_ICCVW_2021_paper.html


There are four parts in this project
## Preprocess
Preprocess the CT-scan volume images: check the image size, extract bounding box and percentage of the the lung in the whole image, select images for 3D CNN

## Segmentation
A UNet segmentation network is trained. It is used to segment lung mask of an image. 

## BERT
A 3D CNN network with BERT for CT-scan volume classification and embedding feature extraction 

## MLP
A simple MLP is trained on the extracted 3D CNN-BERT features. This helps the classification accuracy when there are more than one set of images in a CT-scan volume.  



## License
The code of 3D-CNN-BERT-COVID19 is released under the MIT License. There is no limitation for both academic and commercial usage.

## Citation 

- If you think this work is useful for you, please cite 
 
      @InProceedings{Tan_2021_ICCV,
      author    = {Tan, Weijun and Liu, Jingfeng},
      title     = {A 3D CNN Network With BERT for Automatic COVID-19 Diagnosis From CT-Scan Images},
      booktitle = {Proceedings of the IEEE/CVF International Conference on Computer Vision (ICCV) Workshops},
      month     = {October},
      year      = {2021},
      pages     = {439-445}
      }
   
- This paper has 9 citations as of October 2022, including one paper in Nature Scientific Reports.  
