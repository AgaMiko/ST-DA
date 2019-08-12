
# Improving generalization via style transfer-based data augmentation: Novel regularization method

![Generated skin lesions: an example](https://github.com/AgaMiko/ST-DA/blob/master/Skin-lesions-examples.jpg)

## Introduction
Currently, deep learning (DL) algorithms are considered as state-of-the-art in many classification tasks,
and yet the problem of weak generalization is very common, widely mentioned, and still up-to-date.
One of the main goals in machine learning is to achieve the highest generalization ability of the trained model.
Although huge, multi-layered models are able to extract advanced features from great amounts of data,
unfortunately they often show a tendency to overfit.
The present paper focuses most on the data augmentation. In our method, new images are synthetized with neural style transfer (NST),
and the generated images are then used to train the convolutional neural network (CNN) in order to improve
its generalization abilities.  
The main contributions of this paper are:
*	The proposition of using neural style transfer for the data augmentation technique (ST-DA). This approach is presented on the skin lesion case study by transforming a benign skin lesion to a malignant lesion, and tested with dataset enrichment evaluation; 
*	Incorporating unlabeled, synthesized data into training by adding pseudo-labels generated by another CNN; 
*	Limiting the problem of noisy pseudo-labels in synthetic images used as a CNN training set by using only real images in validation and test sets;
*	Evaluating the ability to enrich the training dataset with artificially generated data with Deep Taylor Decomposition, 
* Proving that the ST-DA method significantly improves the performance and repeatability of training for deep neural networks.


## ST-DA
xxxx
### How-to


### Details
The result and details of the method can be found in the original paper here: [xxx](xxx)
## Database 
### Download
The total databse size is 248 489 unalabeled images (224x224 px). 
Database can be download [here](xxx)
#### If you use this database please star the repository and cite the following paper:
["Improving generalization via style transfer-based data augmentation: Novel regularization method"](xxxx), by [Agnieszka Mikołajczyk](https://scholar.google.pl/citations?user=VFMjpTsAAAAJ&hl=en), [Michał Grochowski](https://scholar.google.pl/citations?user=UTA55L8AAAAJ&hl=en), [Arkadiusz Kwasigroch](https://scholar.google.pl/citations?user=Hw7DV4QAAAAJ&hl=en)

**xxxx

## Sources

The database was generated using following sources:

* *Image generation:*
  * **Style transfer original paper:** [A Neural Algorithm of Artistic Style](https://arxiv.org/abs/1508.06576) is a first paper that presented Neural Style Transfer. 
  * **Style transfer implementation:** Implementation of [Neural Style Transfer & Neural Doodles](https://github.com/titu1994/Neural-Style-Transfer) from the paper A Neural Algorithm of Artistic Style in Keras 2.0+
* *Explaiability method:*
  * **Deep Taylor decomposition:** [DeepTaylor](https://www.sciencedirect.com/science/article/pii/S0031320316303582?via%3Dihub) computes for each neuron a rootpoint, that is close to the input, but which's output value is 0, and uses this difference to estimate the attribution of each neuron recursively.
   * **Repository:** [iNNvestigate](https://github.com/albermax/innvestigate) library contains implementations for the
   SmoothGrad, DeConvNet, Guided BackProp,  PatternNet, DeepTaylor, PatternAttribution, IntegratedGradients and DeepLIFT.  
* *Source database:*
  * **ISIC Archive:** The [ISIC Archive](https://www.isic-archive.com) contains over 23k images of skin lesions, labeled as 'benign' or 'malignant'. Those images were used to generate our database.
  * **ISIC Archive Downloader:** A [script](https://github.com/GalAvineri/ISIC-Archive-Downloader) to download the ISIC Archive of lesion images 
* *Other:*
  * **VGG8** [Selected Technical Issues of Deep Neural Networks for Image Classification Purposes](http://www.czasopisma.pan.pl/Content/112085/PDF/21_363-376_00946_Bpast.No.67-2_28.04.19_K3.pdf) prestents the details of VGG8 architecture.
