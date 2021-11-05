# small-cifar-10
The first 200 image from the [kaggle cifar-10 competition](https://www.kaggle.com/c/cifar-10/overview). The `trainLabel.csv` is Vertex AI manage image dataset format.

## Usage

#### 1. Create a Cloud Storage bucket for our dataset

#### 2. Upload all the image in train folder to the bucket

#### 3. Edit the `trainLabels.csv`
Change the first column to the bucket name you just created

#### 4. Also upload the edited `trainLabels.csv` to Cloud Storage

#### 5. Follow the UI step on Vertex create dataset
- Go the Vertex AI Datesets
- Click create dataset
- Choose `Image classification(Single-label)`
- Choose `Select import files from Cloud Storage`
- Choose the `trainLabels.csv` that we just upload
- Click continue to finish the create dataset process


## contain
The label classes in the dataset are:

- airplane 
- automobile 
- bird 
- cat 
- deer 
- dog 
- frog 
- horse 
- ship 
- truck

## Reference

- [kaggle cifar-10 competition](https://www.kaggle.com/c/cifar-10/overview)
- [Prepare image training data for Vertex AI manage dataset](https://cloud.google.com/vertex-ai/docs/datasets/prepare-image)
