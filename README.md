# HDFENet: High-frequency and Dual-directional Feature Enhancement Network for Maize Tassels Counting
Maize tassels serve as a key indicator for maize yield prediction and breeding evaluation, with their rapid and accurate counting being of great importance to agricultural production. However, existing maize tassels counting methods based on drone image face two persistent challenges: (a) In Convolutional Neural Networks (CNN), downsampling causes loss of high-frequency information.
Leading to the fact that the features of small targets are easily overlooked and resulting in a decline in counting performance; (b) Ineffective utilization of the spatial distribution features of maize tassels leads to background misclassification. To address these limitations, a High-frequency and
Dual-directional Feature Enhancement Network (HDFENet) is proposed. Specifically, an Adaptive High-frequency Feature Enhancement (AHFE) module is developed to mitigate the reduction of edge and texture high-frequency features in CNN. The module extracts frequency-domain features through discrete wavelet decomposition, while utilizing adjacent deep features to generate spatial
masks that dynamically adjust high-frequency features and compensate for detail loss. Furthermore, a Dual-directional Feature Enhancement (DFE) module is introduced to capture the linear spatial distribution of tassels along mechanized planting rows. This module constructs multiscale horizontal and vertical attention maps to precisely capture tassel spatial distribution, thereby reducing target
confusion in dense background scenarios. Experimental validation on a self-constructed maize tassel dataset demonstrates that HDFENet achieves MAE and RMSE values of 10.37 and 12.86, respectively, representing 16.63% and 19.87% improvements over state-of-the-art methods. The proposed HDFENet significantly enhances feature representation and spatial localization of small targets, achieving
optimization in counting accuracy. This method provides an efficient solution for precise maize tassels counting in complex agricultural environments, exhibiting substantial application potential.
![Illustration of the proposed HDFENet. In this architecture, the RGB image is first passed through the encoder to extract features, followed by adaptive high-frequency feature enhancement. It then captures the fine spatial distribution and subsequently inputs it into the regression head for density map generation.](model.png)

## The division of the training set and test set can be found in train.txt and test.txt


## The rest of the code we will open after the article hired

