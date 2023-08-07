# Deploying Custom Sagemaker Containers via GitHub

#### Sagemaker
* fully managed ML service, models can be deployed into production-ready env
* enables distributed training of very Big Data
* integrated Jupyter notebook instance to explore/analyse data
* billed by usage minutes

##### Typical Workflow
* clean/prep data --> train + evaluate model --> deploy model --> generate inferences

###### Training + Evaluation
* Sagemaker has out-of-the-box algorithms for model training (see https://docs.aws.amazon.com/sagemaker/latest/dg/algos.html) e.g., for Image Processing - MXNet, TensorFlow, Semantic Seg
* need to configure compute resources for training - up to cluster of GPUs
* after training, do model evaluation - are inferences OK? Check using AWS SDK in Python (boto) or Sagemaker Python library; use ipynb to train and evaluate model
* ingredients for model training: training data in S3 bucket; ECR path pointing to training code, compute resources, and S3 output path (region of input data and training job must be in same AWS region)
* 

###### Deploy Model (to get inferences)
* usually iterate over model and optimise before integrating with app
* deploy model --> monitor inferences --> collect Ground Truth (GT) --> evaluate model (identify drift)
* increase accuracy by updating training data with collected GT (retraining model)
* deployment depends on use cases:
    - real-time inference for one prediction at a time
    - serverless if OK with cold starts and interim idle periods
    - async inference for large payloads, near real-time latency requirements
    - batch transform for entire dataset
* various ML and Deep learning frameworks e.g., PyTorch, Tensorflow, Scikit-learn, Apache MXNet
    - see Pytorch-Sagemaker Python SDK [guide](https://sagemaker.readthedocs.io/en/stable/frameworks/pytorch/using_pytorch.html#deploy-pytorch-models)


#### Custom Training Containers
* 
* 


#### Integration with GitHub



#### Links
* https://docs.aws.amazon.com/sagemaker/latest/dg/whatis.html
* https://docs.aws.amazon.com/sagemaker/latest/dg/adapt-training-container.html
* https://github.com/aws/amazon-sagemaker-examples/tree/main/advanced_functionality/custom-training-containers
* https://github.com/jlumbroso/free-disk-space



