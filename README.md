# Multimodal_attention_DeepLearning

The multi-modal deep learning algorithm was developed to predict the molecular subtypes of breast cancer. This model was combined with the attention mechanism to create the final model (multi-modal deep learning with intra- and inter-modality attention modules: MDL-IIA)

### Requirements:

* tensorflow-gpu 2.4.0
* numpy 1.19.2
* pandas 1.2.4
* scikit-image 0.18.1
* scikit-learn 0.24.2

### Multimodal_data
Data structure form. CC, craniocaudal (mammography). MLO, mediolateral oblique (mammography). US, ultrasound.

```
.
└── Multimodal_data
    ├── train   
    │     ├── 00001_CC.png
    │     ├── 00001_MLO.png
    │     ├── 00001_US.png
    │     ├── 00002_CC.png
    │     ├── 00002_MLO.png
    │     ├── 00002_US.png
    |     └── ...  
    │
    └── test   
          ├── 00001_CC.png
          ├── 00001_MLO.png
          ├── 00001_US.png
          ├── 00002_CC.png
          ├── 00002_MLO.png
          ├── 00002_US.png
          └── ... 
```

### Model details
Model details of MDL-IIA. a, the proposed multi-modal deep learning with intra- and inter-modality attention model. b, the structure of channel and spatial attention. C, channel. H, height. W, width. Q, query. K, key. V, value. MG, mammography. US, ultrasound. MLO, mediolateral oblique view. CC, craniocaudal view. GAP, global average pooling. FC, fully-connected layer. HER2-E, HER2-enriched. TN, triple-negative.
![image](https://github.com/Netherlands-Cancer-Institute/Multimodal_attention_DeepLearning/blob/main/Model_details.png)
