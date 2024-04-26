# Masked Style-Transfer

The code is based on the [style-transfer-pytorch](https://github.com/crowsonkb/style-transfer-pytorch/tree/master), supporting masked image style transfer.

We also deployed the [**Optimal Transport Loss**](https://aclanthology.org/2022.naacl-main.182.pdf), and a masked seamless clone-style transfer method.

Also, support using a user **word prompt** to mask the given image automatically.

# Usage
Detailed results can be found here:[exp/results.ipynb](https://github.com/wrencanfly/masked-style-transfer/blob/main/exp/results.ipynb)

The main changes happened here: [style_transfer/style_transfer.py](https://github.com/wrencanfly/masked-style-transfer/blob/main/style_transfer/style_transfer.py)


*To enable the mask mode and switch to a different loss function, please follow the comments in the codes.

# Generate an image mask from the user language prompt
Detailed results can be found here: [SAM _generate_mask/predictor_example.ipynb](https://github.com/wrencanfly/masked-style-transfer/blob/main/SAM%20_generate_mask/predictor_example.ipynb)

**User Prompt - "sheep"**
![image](https://github.com/wrencanfly/masked-style-transfer/assets/56505931/0ffd7b40-77ff-4852-9614-1014b0800132)

**User Prompt - "bear"**
![image](https://github.com/wrencanfly/masked-style-transfer/assets/56505931/bfae278e-6ff6-4a6b-86a8-c8de7b230c4e)

**User Prompt - "chair"**
![image](https://github.com/wrencanfly/masked-style-transfer/assets/56505931/cd71ec34-fbf9-43cb-99b6-94cae21f5068)


# Results

- Style Transfer with **Optimal Transport Loss**
  ![1713906422558](https://github.com/wrencanfly/masked-style-transfer/assets/56505931/91743f53-cba4-4ccb-9ce0-2a2c3243f96a)

- **Masked Style Transfer** and Mask Strategies
  ![image](https://github.com/wrencanfly/masked-style-transfer/assets/56505931/b4c8447e-23de-455c-935b-174f4c82b7b6)


- Naive Masekd Style Transfer and Mask Strategies
  ![image](https://github.com/wrencanfly/masked-style-transfer/assets/56505931/8c91dbb1-80d5-4b74-a0f8-a6afae9047f2)

  
- MSE-Style Loss, Wasserstein-2 Loss, and  Optimal Transport Loss
  ![image](https://github.com/wrencanfly/masked-style-transfer/assets/56505931/c28fbf14-96d1-41c8-ba68-ceddc67799fe)




