The project aims to use Pytorch to classify images in CIFAR10 dataset with CNN model

The architecture of CNN is specified as below:
  It contains a BackBone and a Classifier:
    Backbone:
      - Have n number of blocks, each of which contains k number of parallel convolutional layers: 
        + the outputs from parallel structure is combined by a linear equation, where the weights are defined by g(SpatialAveragePool(Input)W) (g is activation function)
    Classifier:
      - Takes as input the output of the last block, then compute the mean feature with Spatial Avg Pool
        + a MLP contains 3 layers
        
=> Result: 87% accuracy
