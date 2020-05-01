## Breast Cancer Pathological Image Classification
G5 - Jeehyun Lee, Yinghan Xu  
For ***"Type-I"*** and ***"Type-II"*** model


### I. Data preparation  
**0_1_Dataset_Maker_BreakHis**  
  : Re-organize BreakHis images for binary class and re-size  
**0_2_Dataset_Maker_BACH**  
  : Re-organize BACH images for binary class and re-size  
**1_Data_Split_BreakHis**  
  : Split data to train, validation, and test sets (80%, 10%, 10%)  

### II. Transfer Learning and Feature extraction  
**2_Transfer_Learning_Bottleneck_Vgg**  
  : Transfer learning using Vgg16  
**3_Transfer_Learning_FineTuning_Vgg**  
  : Fine Tuning  
**4_Vgg_Feature_Extract**  
  : Extract deep features of BreakHis and BACH data from the fine-tuned VGG16   

### III. Combined Model  
**5_Concatenate_Model**  
  : Required to load 'nuclei' data and 'PCA' data  
  https://www.dropbox.com/sh/1c9l05kgbfpazjp/AADCMa6n6VEUiANWhOC8pwPfa?dl=0  

### IV. Test  
**6_Test_BACH**  
