
# Improving generalization via style transfer-based data augmentation: Novel regularization method

![Generated skin lesions: an example](https://github.com/AgaMiko/ST-DA/blob/master/Skin-lesions-examples.jpg)

## Introduction
Currently, deep learning  algorithms are considered as state-of-the-art in many classification tasks,
and yet the problem of weak generalization is very common, widely mentioned, and still up-to-date.

The present paper focuses most on the data augmentation. In our method, new images are synthetized with <em>neural style transfer (NST)</em>,
and the generated images are then used to train the convolutional neural network (CNN) in order to improve
its generalization abilities.  
The main contributions of this paper are:
*	The proposition of using <em>neural style transfer</em> for the data augmentation (ST-DA). This approach is presented on the skin lesion case study by transforming a benign skin lesion to a malignant lesion, and tested with dataset enrichment evaluation; 
*	Incorporating unlabeled, synthesized data into training by adding <em>pseudo-labels</em> generated by another CNN; 
*	Limiting the problem of noisy <em>pseudo-labels</em> in synthetic images used as a CNN training set by using only real images in validation and test sets;
*	Evaluating the ability to enrich the training dataset with artificially generated data with <em>Deep Taylor Decomposition</em>, 
* Proving that the ST-DA method significantly improves the performance and repeatability of training for deep neural networks.


## ST-DA
### How-to
Short and friendly how-to tutorial will be soon available [here](xxx)

### Details
The result and details of the method will be able to be find soon in the original paper here: [xxx](xxx)
You can check instead our previous papers about data augmentation:
  * [Data augmentation for improving deep learning in image classification problem, 2018](https://ieeexplore.ieee.org/abstract/document/8388338)
  * [Style transfer-based image synthesis as an efficient regularization technique in deep learning, 2019](https://arxiv.org/abs/1905.10974)

## Database 
### Download
The total databse size is 248 489 unalabeled images (224x224 px). 
* Full-size examples can be found [here](xxx) (soon)
* Database can be download [soon here](xxx) (soon)
#### If you use this database please star the repository and cite the following paper (soon):
<em> ["Improving generalization via style transfer-based data augmentation: Novel regularization method"](xxxx)</em>, by [Agnieszka Mikołajczyk](https://scholar.google.pl/citations?user=VFMjpTsAAAAJ&hl=en) , [Michał Grochowski](https://scholar.google.pl/citations?user=UTA55L8AAAAJ&hl=en), [Arkadiusz Kwasigroch](https://scholar.google.pl/citations?user=Hw7DV4QAAAAJ&hl=en)

## Sources

The database was generated using following sources:

* *Image generation:*
  * **Style transfer original paper:** [A Neural Algorithm of Artistic Style](https://arxiv.org/abs/1508.06576) is a first paper that presented <em>Neural Style Transfer</em>. 
  * **Style transfer implementation:** Implementation of [Neural Style Transfer & Neural Doodles](https://github.com/titu1994/Neural-Style-Transfer) from the paper <em>A Neural Algorithm of Artistic Style</em> in Keras 2.0+
* *Explainability method:*
  * **Deep Taylor decomposition:** [DeepTaylor](https://www.sciencedirect.com/science/article/pii/S0031320316303582?via%3Dihub) computes for each neuron a rootpoint, that is close to the input, but which's output value is 0, and uses this difference to estimate the attribution of each neuron recursively.
   * **Repository:** [iNNvestigate](https://github.com/albermax/innvestigate) library contains implementations for the
   SmoothGrad, DeConvNet, Guided BackProp,  PatternNet, DeepTaylor, PatternAttribution, IntegratedGradients and DeepLIFT.  
* *Source database:*
  * **ISIC Archive:** The [ISIC Archive](https://www.isic-archive.com) contains over 23k images of skin lesions, labeled as 'benign' or 'malignant'. Those images were used to generate our database.
  * **ISIC Archive Downloader:** A [script](https://github.com/GalAvineri/ISIC-Archive-Downloader) to download the ISIC Archive of lesion images 
* *Previous papers about data augmentation:*
  * [Data augmentation for improving deep learning in image classification problem, 2018](https://ieeexplore.ieee.org/abstract/document/8388338)
  * [Style transfer-based image synthesis as an efficient regularization technique in deep learning, 2019](https://arxiv.org/abs/1905.10974)
* *Similar projects:*
  * **Generating skin lesions with GANs** - [Beating Melanoma with Deep Learning: letting the data speak](https://github.com/devansh20la/Beating-Melanoma/tree/master/Generator)
* *Other:*
  * **VGG8** [Selected Technical Issues of Deep Neural Networks for Image Classification Purposes](http://www.czasopisma.pan.pl/Content/112085/PDF/21_363-376_00946_Bpast.No.67-2_28.04.19_K3.pdf) prestents the details of VGG8 architecture.
