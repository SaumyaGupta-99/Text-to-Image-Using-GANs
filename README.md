# Text-to-Image-Using-GANs
Code for ATTGAN And DM-GAN for conversion of text into images using Caltech bird Dataset.

<h3>ATTGAN</h3>
AttGAN is a useful GAN model that allows attention-driven, multi-stage refinement for fine-grained text-to-image generation. This model addresses the problem that in most of the approaches whole text sentence is converted into a global sentence vector that is then fed to the GAN network. The global sentence vectors prevent generation of high quality images as they lack important fine grained information at word level. AttGAN model consists of two novel components. First one is an
attentional generative network in which generator draws different sub regions of image by focusing on words that are most relevant to sub region being drawn.Another component is Deep Attentional Multimodal Similarity Model (DAMSM). DAMSM compares the generated image with text using both global word level information and fine grained word level information.
 
<h3>DMGAN</h3>
Dynamic Memory Generative Adversarial Networks was developed to address two issues - results generated depend largely on the quality of initial images and each word in an input text provides different level of information depicting the image content. The current models are not able to properly deal with such issues. DM-GAN[8] deals with the such issue by providing a memory mechanism to cope up with badly generated images. Inspired by the memory network’s ability to encode knowledge sources key-value memory structures have been addedto GAN network.A response gate has also been proposed to adaptively fuse information from image and memory. Many experiments propose that this method beats many of the state of art methods.

<h3>About DataSet</h3>
I would be using Caltech-UCSD Birds 200 (CUB-200) [10] for my project. CUB dataset is a large scale
dataset aimed at subordinate categorization which has 6,033 annotated images of birds classified into
200 categories. I would be using meta data of this dataset has well which includes captions for each of
the images in a pickle file.
  
<h3>Methods for Performance Evaluation</h3>
- Inception Score  - R precision  - Using TSNE to reduce image feature dimensionalities to plot them to compare how close are images generated by GANs to the image output available in test set.
