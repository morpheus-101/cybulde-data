# Hate speech detection

## Overview
This project aims to detect and classify hate speech, toxic comments, and cyberbullying content using machine learning techniques. It utilizes a combination of publicly available datasets to train and evaluate the models. Distributed data preprocessing, distributed model training, dataset and model deployment, model monitoring all done on Google Cloud Platform. 

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
