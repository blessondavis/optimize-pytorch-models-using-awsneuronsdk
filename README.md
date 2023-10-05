# Optimize Pytorch Models Using AWS Neuron SDK

In this tutorial, we'll deploy a pre-trained BERT Base model from HuggingFace Transformers on SageMaker using AWS Deep Learning Containers. 

The model will be compiled using the Neuron SDK, and a customized AWS Deep Learning Container will be constructed, integrating the HuggingFace Transformers Library. 
A list of containers can be found here: https://github.com/aws/deep-learning-containers/blob/master/available_images.md#sagemaker-framework-containers-sm-support-only

After compiling the model using Neuron SDK (neuron-cc), we can deploy the model on Amazon Inferentia1 Instances.

I ran this Jupyter Notebook on a ml.c5.4xlarge SageMaker Notebook instance (not Sagemaker Studio). 

You can read more about Neuron SDK here and how to extend this approach for Tensorflow and MXNet frameworks as well: https://awsdocs-neuron.readthedocs-hosted.com/en/latest/index.html

