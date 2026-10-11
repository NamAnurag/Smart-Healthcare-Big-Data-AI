# Smart Healthcare with Big Data & AI

An end-to-end healthcare IoT analytics project combining exploratory data analysis, machine learning, big-data processing, patient monitoring profiles, and Generative AI-assisted explanations.

## Project Overview

This project analyzes multi-sensor healthcare IoT data to explore patient monitoring patterns, study activity classification, investigate fall-related signals, and group sensor observations into data-driven monitoring profiles.

It combines Python-based analytics with PySpark processing and AWS integration concepts to demonstrate how healthcare data can be processed and analyzed at scale.

## Key Features

- **Exploratory Data Analysis:** Examines sensor distributions, missing values, duplicates, and activity patterns.
- **Activity Classification:** Uses Decision Tree and Random Forest models to study activity-related patterns.
- **Feature Importance:** Identifies features contributing to the activity classification models.
- **Big Data Processing:** Uses PySpark to aggregate healthcare sensor measurements and analyze activity patterns.
- **Healthcare Monitoring Profiles:** Applies K-Means clustering to group observations based on selected sensor features.
- **Interactive Monitoring Dashboard:** Accepts sensor inputs and assigns them to a learned monitoring profile.
- **Generative AI Integration:** Develops prompts for patient-friendly explanations of monitoring profiles.
- **Security Analysis:** Includes a STRIDE-based threat-modeling section for the healthcare data workflow.

## Technology Stack

- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn
- PySpark
- AWS S3
- AWS Bedrock integration
- Google Colab
- Jupyter Widgets

## K-Means Clustering

The final clustering workflow uses five selected features:

- Heart rate
- SpO₂ level
- Blood glucose
- Stress level index
- Step count

The features are standardized using `StandardScaler`. The final K-Means model uses 12 clusters, `random_state=42`, and `n_init=30`.

The notebook reports a silhouette score of approximately **0.1999** for the selected-feature clustering workflow. This indicates limited separation between some clusters, so the profiles should be interpreted as exploratory groupings rather than clinical diagnoses.

## Dataset

The project uses a multi-sensor medical IoT dataset containing physiological measurements, activity information, and related sensor readings.

The dataset itself is not included in this repository. Users must obtain authorized access to the dataset before running the complete notebook.

## How to Run

1. Open the notebook in this repository.
2. Select **Open in Colab**, or download the `.ipynb` file and open it in Jupyter.
3. Obtain the required dataset and configure the input path.
4. Install any missing dependencies.
5. Configure AWS credentials securely if running the AWS integration cells.
6. Execute the notebook cells in order.

Some cells require Google Colab, an authorized dataset, AWS permissions, or access to an appropriate Generative AI model. These integrations may need configuration before they can run in another environment.

## Project Limitations

- The clustering profiles are exploratory and are not medical diagnoses.
- Model performance depends on the dataset, selected features, and validation method.
- AWS and Generative AI integrations require appropriate configuration and permissions.
- Results should not be used as a substitute for professional medical evaluation.

## Author

**Anurag Gupta**

B.Tech, Computer Science and Engineering

GitHub: [NamAnurag](https://github.com/NamAnurag)

---

*Academic project exploring healthcare IoT analytics, machine learning, big-data processing, and AI-assisted monitoring.*
