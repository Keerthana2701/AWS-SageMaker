# AWS-SageMaker

-- AWS SageMaker is a cloud ML Platform
-- Use Amazon Sagemaker Studio or Create Notebook instances

## Two components are present in Amazon SageMaker: 
-- Model training 
-- Model deployment

##  Model training and Deployment :


Create SageMaker session
Create execution role (IAM) for notebook instance
Cnvert the data in numpy array format to RecordIO format since Sagemaker needs data in this format
Amazon S3 bucket URL (training data): where the training data is located.
Compute resources: Amazon SageMaker will train the model using instances managed by Amazon SageMaker.
Get training container of sagemaker built in algorithms by giving the PCA container image
Amazon S3 bucket URL (Output): this bucket will host the output from the training.
Amazon Elastic Container Registry path: where the training code is stored. 
Amazon SageMaker launches an ML compute instances once a training job is initiated. 
Amazon SageMaker uses: (1) training code and (2) training dataset to train the model. 
Amazon SageMaker saves the trained model artifacts in an S3 bucket.

Pass the output path, instance type, container and instance count in the estimator and tune hyperparameters for training 
Deploy the model to perform inference

Train and evaluate the XGBoost model on data obtained after PCA.



