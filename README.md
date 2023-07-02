# VGGEntropyKernelGraphCut-Paper-With-Code
Textural Image Segmentation based on Entropy and VGG16 Deep Neural Network Kernel Graph Cut

This repository presents an enhanced approach to the entropy-based graph cut algorithm for image segmentation by incorporating a feature space extracted from the VGG16 deep neural network. By introducing this additional feature space, the effectiveness of the graph cut algorithm kernel for pixel segmentation is improved.

The integration of the VGG16 deep neural network in the proposed algorithm provides valuable image features for improved segmentation performance. The VGG16 network, pre-trained on a large-scale dataset, has demonstrated strong capabilities in extracting hierarchical and discriminative features from images. By incorporating the VGG16 feature space, the algorithm benefits from the learned representations that capture both low-level and high-level visual information. These features, combined with the entropy-based kernel graph cut approach, enhance the algorithm's ability. In the weighted kernel graph cut algorithm, based on entropy and VGG16, the centers for the background and foreground regions are determined using a weighted k-means algorithm. The RBF kernel is then fine-tuned to implicitly map the data to the higher-dimensional space based on these centers. After extracting the pixel weights from the image, they are utilized to extract the weighted centers in the k-means algorithm, taking into account the importance of each pixel. Data points are assigned to the nearest cluster center based on their membership degree. New cluster centers are then calculated for each cluster based on the membership degree and pixel weights. After obtaining the kernel output, the data term based on the kernel components and the regularization term based on the calculated averages are computed. The energy function is determined by combining these two components, and an image graph is constructed based on the energy function.

If you find this work useful in your research, please consider citing the following paper:

M. Niazi, K. Rahbar, M. Sheikhan, and M. Khademi, "Textural Image Segmentation based on Entropy and VGG16 Deep Neural Network Kernel Graph Cut," Adv. Signal Process., May 2023.

You can access the paper at https://jasp.tabrizu.ac.ir/article_16328.html?lang=en 
