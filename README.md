# Brain Cancer Medical Imaging Classification

<a target="_blank" href="https://cookiecutter-data-science.drivendata.org/">
    <img src="https://img.shields.io/badge/CCDS-Project%20template-328F97?logo=cookiecutter" />
</a>
<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/87e4f1bc-8392-4655-93fb-dc3227a54d07" />
AI generated image

# Introduction
Cancer remains one of the leading causes of death worldwide, responsible for approximately 10 million deaths annually (Gou X, 2025). Alarmingly, 70% of cancer deaths are accounted by low and mid income countries. This is primarily because of limited access to screening, diagnosis, treatment, and palliative care (Oghenekaro, 2025). Cancer can be seen as not only a medical challenge, but also a socioeconomic one. To make healthcare outcome more equitable, novel innovations in AI can be utilized for early detections in improving survival outcomes for patients.

DL learning, a subset of machine learning, is the revolutionary machine learning architecture spearheading the innovation in early cancer detection for improved prognosis. Utilizing convolutional neural networks, machine learning algorithms learn end-to-end complex features in medical images that are relevant to an image classification or an object detection problem. Such advancement increases societal health outcomes by enabling accelerated and accurate medical image interpretation and analysis. This is especially helpful in low and mid income countries where there is inadequate screening infrastructure.

In this project we will be working with the Bangladesh Brain Cancer MRI dataset. The dataset is a comprehensive collection of brain MRI images meticulously sourced from various hospitals in Bangladesh on three brain cancer types: meningioma, glioma, and pituitary tumor. Utilizing this data we will train a neural network classifier and answer the following research questions:

- What level of performance can be reached with an end-to-end neural network utilizing a moderate sample size?
- Which neural network architecture is most performant and why?

# Data Provenance
The data was sourced from Mendely.com, which is an open-source repository where researchers publish their datasets. The dataset retrieved from this repository was the Bangladesh Brain Cancer MRI dataset. It contains 6056 images of systemically categorized MRI images of three distinct cancer classes. The purpose of utilizing this dataset was to create a prototype of a tool that healthcare professionals could utilize for augmenting MRI image interpretation for improved patient outcomes. The specific research questions asked in the project were: “Which neural network architecture is most performant for cancer imaging classification and why?” and ”What level of performance can be reached with an end-to-end neural network utilizing a moderate sample size?”. 

# Key Findings
Utilizing a custom-built ResNet the model was able to achieve remarkable discriminatory performance. The highest performing model achieved a balanced accuracy of 93%, which is a 19% increase in the balanced accuracy of the baseline model. The quality of the classifier was evaluated with a one-versus-all ROC curve. The AUC statistic across all three classes was greater than 0.90, indicating an excellent discriminatory performance. The highest AUC statistic achieved was 0.98 for the “brain_glioma” class, while the lowest AUC statistic was 0.92 for the “brain_menin” class. This demonstrated the model's strong performance in capturing true positive instances across classification thresholds, keeping false positives to a minimum. Moving to the classification report, the F1-score for all three classes demonstrated superb harmonic balance between recall and precision. The F1-Score ranged from 0.93 – 0.96. In regard to the precision and recall, the model reports robust performance. The recall statistics for the classes “brain_glioma”, “brain_menin”, and “brain-tumor” were 0.99, 0.84, and 0.98, respectively. This information conveys that the model does an excellent job at capturing true positive instances in its predictions. This is critical in a high-stakes environment where misclassification can lead to misdiagnosis and decreased survival time. The precision statistics for the classes “brain_glioma”, “brain_menin”, and “brain-tumor” were 0.93, 0.99, and 0.89, respectively. These strong precision metrics reveal that, given a positive prediction, there is a high probability that the patient actually has the disease. 

Overall, the strong performance demonstrates the potential for AI in medical imaging interpretation. Computer vision in medical imaging for cancer can facilitate faster, accurate, and reliable interpretation of medical images. This will allow more individuals to get screened, diagnosed, and receive early treatment for improved survival probabilities and better quality of life. 

# Project Artifacts
<img width="605" height="531" alt="image" src="https://github.com/user-attachments/assets/f851df08-7a8f-4bdc-809a-000064af73d9" />
One-versus-all ROC curve for the highest performing model


## Project Organization

```
├── LICENSE            <- Open-source license if one is chosen
├── README.md          <- The top-level README for developers using this project.
│
├── notebooks          <- HTML Jupyter notebook. Naming convention is a number (for ordering),
│                         the creator's initials, and a short `-` delimited description, e.g.
│                         `1.0-jqp-initial-data-exploration`.
│
│
├── references         <- Data dictionaries, manuals, and all other explanatory materials.
