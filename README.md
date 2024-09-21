# Inception-from-Scratch-in-Pytorch
The following python notebook shows the ptyorch code of  googleNet popularly known as Inception Network, which is widely used in the field of Computer Vision, from scratch.


## Why Inception?

### 1. Multiple features at each Layer -
this is used to capture features at different spatial scales.
The outputs of all these operations are concatenated, allowing the network to learn a rich combination of features.

**Why it matters?** This multi-scale approach gives the network the ability to adapt and capture more relevant features without needing to decide a priori the best filter size for a given feature map.

### 2. 1x1 Convolutions for Dimensionality Reduction -
Without this, larger filters (like 5x5) would greatly increase the number of parameters and the computation load.

**Why it matters?** This allows the network to be deep and wide while maintaining computational feasibility, and it introduces more non-linearity to the model.

### 3. Parallelism and Efficiency:
By combining operations of different filter sizes in parallel, the network learns in a more structured, hierarchical manner, efficiently processing different scales and types of features. Inception networks are able to increase depth (layers) and width (features) without exponentially increasing the number of parameters.

#### This makes Inception networks ideal for real-world applications where computational resources might be limited, but high performance is still necessary.
