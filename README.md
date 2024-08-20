# Cyber bullying detection

## 📚 Project Overview
This project is focused on developing a deep learning model to detect and classify hate speech, toxic comments, and cyberbullying content on online platforms. The key goal is to create a robust, scalable, and reproducible MLOps pipeline for building and serving deep learning projects to the cloud.

*Note: The objective of this project is to design and implement an MLOps pipeline on the cloud, tailored for a deep learning application. While the current text classification model—a fine-tuned BERT-based model—serves as a foundational example, it is acknowledged that this may not be the most optimal solution for the problem at hand. However, the developed infrastructure is fully capable of supporting more advanced and high-performing models. This infrastructure is not only directly applicable to building better models but also serves as a versatile template for developing and deploying a wide range of deep learning applications.*

🛠️ Ensuring Reproducibility and Maintainability
- **Docker Containerization**: Packages the project, including dependencies, into a Docker container for consistent cross-platform deployment.
- **Data Version Control with DVC**: Manages dataset changes with DVC, enabling reproducible experiments and seamless model retraining.
- **Distributed Data Processing with Dask**: Uses Dask for efficient, scalable data preprocessing and feature engineering.
- **Distributed Model Training with PyTorch**: Accelerates training with PyTorch's distributed capabilities, utilizing multiple GPUs or CPU cores.
- **Cloud-based Infrastructure**: Deployed on Google Cloud Platform (GCP), utilizing its scalable infrastructure, secure storage, Docker management, and Mlflow for model tracking.
- **Configuration Management with Hydra**: Employs Hydra-core for streamlined configuration management and enhanced reproducibility.

The project is divided into four parts(each in its own repo):
- Part 1: [Data collection and versioning]()
- Part 2: [Distributed data processing]()
- Part 3: [Distributed model training and evaluation]()
- Part 4: [Deployment and web app]()

This repository includes code for Part 1 only. 

---

# Part 1:

## Tools and Technologies
- **DVC (Data Version Control)**: DVC is used for data versioning, allowing the team to track changes in the dataset over time and reference specific versions using Git tags.
- **Google Cloud Storage (GCS)**: The dataset is stored in a GCS bucket, providing a reliable and scalable remote storage solution for the versioned data.
- **GitHub**: GitHub is used for version control of the project code and to store the metadata and tags associated with the versioned datasets.

## Approach overview: 
- The project uses DVC for data versioning and GCS for remote storage of the datasets. The versioning information is stored on GitHub using Git tags, allowing to reference specific versions of the datasets.
To fetch a specific version of the dataset, use the corresponding Git tag.

## Datasets
The project utilizes the following datasets:
1. **GAB Hate Corpus**: The GHC, which is the largest theoretically-justified, annotated corpus of hate speech to date, provides opportunities for training and evaluating hate speech classifiers and for scientific inquiries into the linguistic and network components of hate speech. [Link](https://osf.io/edua3/)
2. **Toxic Comments Classification Challenge**: A dataset with a large number of Wikipedia comments which have been labeled by human raters for toxic behavior. The types of toxicity are: toxic, severe_toxic, obscene, threat, insult, identity_hate [Link](https://www.kaggle.com/c/jigsaw-toxic-comment-classification-challenge)
3. **Cyberbullying Tweets Dataset**: A dataset of tweets labeled as either cyberbullying or non-cyberbullying. [Link](https://www.kaggle.com/datasets/saurabhshahane/cyberbullying-dataset)

## Credits

