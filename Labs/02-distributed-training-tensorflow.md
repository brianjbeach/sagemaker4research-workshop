# Distributed Training with TensorFlow 

In this lab we will be using images of handwritten digits from the [MNIST Database](http://yann.lecun.com/exdb/mnist/) to demonstrate how to perform distributed training using SageMaker. Using a convolutional neural network model based on the [TensorFlow MNIST Example](https://github.com/tensorflow/models/tree/master/official/mnist), we will demonstrate how to use a Jupyter notebook and the [SageMaker Python SDK](https://github.com/aws/sagemaker-python-sdk) to create your own script to pre-process data, train a model, create a SageMaker hosted endpoint, and make predictions against this endpoint. The model will predict what the handwritten digit is in the image presented for prediction. Besides demonstrating a "bring your own script" for TensorFlow use case, the example also showcases how easy it is to set up a cluster of multiple instances for model training in SageMaker.

1. In your notebook instance, click on the `SageMaker Samples` tab.
2. Open the `tensorflow_distributed_mnist.ipynb` notebook from the `Sagemaker Python Sdk` section.
3. Follow the directions in the notebook.

<p><strong>NOTE:  training the model for this example typically takes about 8 minutes.</strong></p>

## Extra Credit

1. How would a GPU change training time?  Rather than training on two ml.c4.xlarge try training with one ml.p2.xlarge.
2. Sometimes you don't need a cluster for training. You can train your model on the notebook instance. Try running the `tensorflow_local_mode_mnist.ipynb` notebook.
3. Rather than configuring an endpoint for real time inference, you may want to process a large batch of samples. Try running the `tensorflow_batch_transform_mnist.ipynb` notebook.
