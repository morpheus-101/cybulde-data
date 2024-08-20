# Hate speech and Toxicity detection

## Overview
This project is focused on developing advanced machine learning models to detect and classify hate speech, toxic comments, and cyberbullying content from online platforms. By leveraging a diverse set of publicly available datasets, our goal is to create robust and accurate models that can help combat the growing problem of online toxicity and harassment.

Ensuring Reproducibility and Maintainability
- Docker Containerization: The entire project, including its dependencies and runtime environment, is packaged into a Docker container. This ensures that the application can be consistently deployed and executed across different platforms, eliminating the risk of environmental discrepancies.
- Data Version Control with DVC: The project utilizes DVC (Data Version Control) to manage and track changes in the dataset over time. This allows the team to reference specific versions of the data, enabling reproducible experiments and facilitating seamless model retraining as new data becomes available.
- Distributed Data Processing with Dask: The preprocessing of the large datasets is handled using the Dask distributed computing framework. This enables efficient data transformation and feature engineering, ensuring scalability and optimizing resource utilization.
- Distributed Model Training with PyTorch: The model training process is parallelized using PyTorch's distributed training capabilities, leveraging multiple GPUs or CPU cores to accelerate the training process and improve model performance.
- Cloud-based Infrastructure: The project is deployed and managed on the Google Cloud Platform (GCP), taking advantage of its robust and scalable infrastructure. This includes the use of Google Cloud Storage for secure data storage, Google Artifact Registry for Docker image management, and Mlflow for comprehensive model tracking and performance evaluation.

The project is divided into four parts:
- Part 1: [Data collection and versioning]()
- Part 2: [Distributed data preparation]()
- Part 3: [Distributed model training and evaluation]()
- Part 4: [Deployment and web app]()

This repository includes code for Part 1 only. 

## Tools and Technologies
- **Docker**: The project is set up to run within a Docker container, ensuring a consistent and reproducible environment.
- **DVC (Data Version Control)**: DVC is used for data versioning, allowing the team to track changes in the dataset over time and reference specific versions using Git tags.
- **Google Cloud Storage (GCS)**: The dataset is stored in a GCS bucket, providing a reliable and scalable remote storage solution for the versioned data.
- **GitHub**: GitHub is used for version control of the project code and to store the metadata and tags associated with the versioned datasets.

## Datasets
The project utilizes the following datasets:
1. **GAB Hate Corpus**: The GHC, which is the largest theoretically-justified, annotated corpus of hate speech to date, provides opportunities for training and evaluating hate speech classifiers and for scientific inquiries into the linguistic and network components of hate speech. [Link](https://osf.io/edua3/)
2. **Toxic Comments Classification Challenge**: A dataset with a large number of Wikipedia comments which have been labeled by human raters for toxic behavior. The types of toxicity are: toxic, severe_toxic, obscene, threat, insult, identity_hate [Link](https://www.kaggle.com/c/jigsaw-toxic-comment-classification-challenge)
3. **Cyberbullying Tweets Dataset**: A dataset of tweets labeled as either cyberbullying or non-cyberbullying. [Link](https://www.kaggle.com/datasets/saurabhshahane/cyberbullying-dataset)

## Data Versioning and Storage
The project uses DVC for data versioning and GCS for remote storage of the datasets. The versioning information is stored on GitHub using Git tags, allowing to reference specific versions of the datasets.

To fetch a specific version of the dataset, you can use the corresponding Git tag.

## Credits

## License
This project is licensed under the [MIT License](LICENSE).
