Using AWS SageMaker/PlanesNet to process Satellite Imagery  
===========================================

This solution shows how to process satellite imagery using AWS SageMaker and PlanesNet to build an AI Model to predict aircraft. This readme updates an article "Detect airplanes in Planet imagery using machine learning" by Bob Hammell referenced below and provides a more basic step by step process.

We'll start a Jupyter Notebook using AWS SageMaker.  We can then use the Jupyter Notebook to process all the steps required to predict aircraft in the satellite imagery.


## Configure AWS SageMaker
Use the AWS Console to configure a SageMaker Instance for processing satellite data.  This is a step by step process.

### AWS SageMaker Dashboard
Click on "Notebook instances"  
Click on "Create notebook instance"  
Notebook instance name: planesnet  
Notebook instance type: ml.t2.medium   
IAM Role: Create a new role  
```
S3 buckets you specify - optional:
Select "None"
Click on "Create role"
```
Click on "Create notebook instance"

#### Display Notebook instances using the SageMaker Dashboard
Notebook/Notebook instances  
Name: planesnet  
Actions: Open  # it will show pending until it's ready to open

This will open the Jupyter Notebook in a new tab in your browser.

#### Upload aws-sagemaker-planesnet.ipynb using Jupyter Notebook
Click on "Upload" and Select "aws-sagemaker-planesnet.ipynb" from project jupyter-notebook directory 

Once the notebook is uploaded, click on "aws-sagemaker-planesnet.ipynb" to open it.  
Run each cell Step by Step

## References
Detect airplanes in Planet imagery using machine learning  
https://github.com/rhammell/planesnet-detector