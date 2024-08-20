# Project Title

## Description
This project aims to detect and classify hate speech, toxic comments, and cyberbullying content using machine learning techniques. It utilizes a combination of publicly available datasets to train and evaluate the models.

## Tools and Technologies
- **Docker**: The project is set up to run within a Docker container, ensuring a consistent and reproducible environment.
- **DVC (Data Version Control)**: DVC is used for data versioning, allowing the team to track changes in the dataset over time and reference specific versions using Git tags.
- **Google Cloud Storage (GCS)**: The dataset is stored in a GCS bucket, providing a reliable and scalable remote storage solution for the versioned data.
- **GitHub**: GitHub is used for version control of the project code and to store the metadata and tags associated with the versioned datasets.

## Datasets
The project utilizes the following datasets:
1. **GAB Hate Corpus**: A dataset of hate speech collected from the social media platform Gab. [Link](https://osf.io/edua3/)
2. **Toxic Comments Classification Challenge**: A dataset of comments from Wikipedia's talk page edits, labeled for various toxicity types. [Link](https://www.kaggle.com/c/jigsaw-toxic-comment-classification-challenge)
3. **Cyberbullying Tweets Dataset**: A dataset of tweets labeled as either cyberbullying or non-cyberbullying. [Link](https://www.kaggle.com/datasets/saurabhshahane/cyberbullying-dataset)

## Data Versioning and Storage
The project uses DVC for data versioning and GCS for remote storage of the datasets. The versioning information is stored on GitHub using Git tags, allowing the team to reference specific versions of the datasets.

To fetch a specific version of the dataset, you can use the corresponding Git tag.

## Contributing
Contributions to this project are welcome. Please follow the steps outlined in the [Contributing](#contributing) section of the README.

## License
This project is licensed under the [MIT License](LICENSE).
