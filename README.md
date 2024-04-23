# Masked Style-Transfer

The code is based on the [style-transfer-pytorch](https://github.com/crowsonkb/style-transfer-pytorch/tree/master), supporting masked image style transfer.

We also deployed a new **Optimal Transport Loss**, and a masked seamless clone-style transfer method.

# Usage
Detailed results can be found here:[exp/results.ipynb](https://github.com/wrencanfly/masked-style-transfer/blob/main/exp/results.ipynb)

The main changes happened here: [style_transfer/style_transfer.py](https://github.com/wrencanfly/masked-style-transfer/blob/main/style_transfer/style_transfer.py)


*To enable the mask mode and switch to a different loss function, please follow the comments.


# Results

- Style Transfer with **Optimal Transport Loss**
  ![1713906422558](https://github.com/wrencanfly/masked-style-transfer/assets/56505931/91743f53-cba4-4ccb-9ce0-2a2c3243f96a)

- **Masked Style Transfer** and Mask Strategies
  ![image](https://github.com/wrencanfly/masked-style-transfer/assets/56505931/b4c8447e-23de-455c-935b-174f4c82b7b6)


- Naive Masekd Style Transfer and Mask Strategies
  ![image](https://github.com/wrencanfly/masked-style-transfer/assets/56505931/8c91dbb1-80d5-4b74-a0f8-a6afae9047f2)

  
- MSE-Style Loss, Wasserstein-2 Loss, and  Optimal Transport Loss
  ![image](https://github.com/wrencanfly/masked-style-transfer/assets/56505931/c28fbf14-96d1-41c8-ba68-ceddc67799fe)




