# Generate-synthetic-data
# Overview
This project demonstrates a workflow for generating synthetic data focused on rare events using a Variational Autoencoder (VAE). It is designed to augment small, scarce datasets common in domains like anomaly detection, healthcare, and finance by producing realistic synthetic samples for improved machine learning performance.

# Installed Libraries
This project depends on the following Python packages:

- pandas

- numpy

- scikit-learn

- matplotlib

- seaborn

- tensorflow

They can be installed using:


    pip install pandas numpy scikit-learn matplotlib seaborn tensorflow

# What i built ?
 - A Python-based pipeline that:
   
    - Loads an existing rare event CSV dataset or creates a dummy dataset if the file is missing.
    - Preprocesses the data by imputing missing values, scaling numerical features, and encoding categorical features.
    - Defines and trains a VAE model on the preprocessed data.
    - Generates synthetic data samples via the trained VAE decoder.
    - Compares synthetic and original data using visualization and statistics for quality evaluation.

# Why i built it ?
Rare event data is often insufficient for building effective models due to its scarcity. This project addresses the challenge of data scarcity by generating high-quality synthetic data that resembles the original rare event distribution, facilitating robust model training, evaluation, and experimentation.

# How i built it ?
- Used Python libraries such as pandas and numpy for data handling and preprocessing.

- Employed scikit-learn's tools for scaling and encoding features.

- Implemented the VAE in TensorFlow/Keras, designing encoder and decoder architectures compatible with tabular data.

- Trained the model with appropriate loss functions and optimization steps.

- Generated synthetic samples through random latent space sampling and decoded them to tabular form.

- Visualized differences and refined the model iteratively based on statistical comparisons.

# Conclusion
Synthetic data generation using VAEs provides a promising approach to augment limited rare event datasets. By creating realistic synthetic samples, this method enables improved robustness and reliability in machine learning models trained on scarce data. This workflow serves as a foundation for ongoing refinement and adaptation to various rare event scenarios.
