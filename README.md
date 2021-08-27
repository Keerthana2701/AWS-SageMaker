# AWS-SageMaker

-- AWS SageMaker is a cloud ML Platform
-- Use Amazon Sagemaker Studio or create Notebook instances

## Two components are present in Amazon SageMaker: 
-- Model training 
-- Model deployment

##  Model training and Deployment for Cardiovascular disease prediction:


 Create SageMaker session <br /> 
 Create execution role (IAM) for notebook instance <br />
Cnvert the data in numpy array format to RecordIO format since Sagemaker needs data in this format <br />
Amazon S3 bucket URL (training data): where the training data is located. <br />
Compute resources: Amazon SageMaker will train the model using instances managed by Amazon SageMaker. <br />
Get training container of sagemaker built in algorithms by giving the PCA container image <br />
Amazon S3 bucket URL (Output): this bucket will host the output from the training. <br />
Amazon Elastic Container Registry path: where the training code is stored.  <br />
Amazon SageMaker launches an ML compute instances once a training job is initiated. <br />
Amazon SageMaker uses: (1) training code and (2) training dataset to train the model. <br />
Amazon SageMaker saves the trained model artifacts in an S3 bucket. <br />

Pass the output path, instance type, container and instance count in the estimator and tune hyperparameters for training <br />
Deploy the model to perform inference <br />

Train and evaluate the XGBoost model on data obtained after PCA. <br />



