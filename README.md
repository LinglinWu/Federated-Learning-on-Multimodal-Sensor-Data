# Project Title
Federated-Learning-on-Multimodal-Sensor-Data

## Motivation
The goal of federated learning is to collaboratively train a machine learning model
where the participating parties wish to keep their data private. Data can be of different modalities,
i.e., can be images, audio, text, sensor data etc. Recently, there have been works in the field of
multimodal federated learning. A variety of heterogeneous sensor deployments with multiple
sensing modalities are emerging that serve a single learning application. The sensor data is private
in nature and requires federated learning approach, hence the demand for multimodal FL in
research community is increasing.

## Design Goals
Understand and benchmark different multimodal datasets in a federated setting

## Deliverables
Understand multimodal federated learning (code:https://github.com/yuchenzhao/iotdi22-mmfl)
Use given datasets to reproduce the results in the paper data: https://drive.google.com/drive/folders/1rWJYkfMavGs1F-H0jykJ5V0fIiwrQdJV
Perform a per-class accuracy analysis of the results and observe the effect of skewed data distribution on the per-class accuracy
Evaluate the system on a multimodal dataset that is relatively balanced in class distribution

## System Blocks
   [Sensor Data Sources]
            ↓
    [Data Preprocessing]
            ↓
    [Local Device Processing]
          (Client Devices)
  ┌──────────────┐         ┌──────────────┐
  │ Client 1     │  ...    │ Client N     │
  │ - Model Train│         │ - Model Train│
  │ - Update     │         │ - Update     │
  └──────────────┘         └──────────────┘
            ↓
     [Federated Aggregator]
            ↓
       [Global Model Update]
            ↓
     [Evaluation and Analysis]
            ↓
       [Results and Analysis]


## HW/SW Requirements

**Software Requirements:**
Python, Laptop with CUDA-enabled GPU (optional)

## Team Members Responsibilities
| Name       | Role               |
|------------|---------------------|
| Linglin Wu | Lead Researcher & Model Developer  |
| Rui Li     | System Integrator & Documentation Specialist   |


## Project Timeline
| Milestone  | Start Date | End Date | Description              |
|------------|------------|----------|--------------------------|
| Data Preparation    | 10/01/2024 | 10/10/2024 | Collect and preprocess multimodal sensor data. Ensure data is cleaned and normalized for training.          |
| Implementation Setup    | 10/11/2024 | 10/20/2024 | Set up the federated learning environment, install required software, and ensure GPU compatibility.          |
| Initial Model Training    | 10/21/2024 | 10/31/2024 | Train the initial model on local devices using the multimodal sensor data. Validate data flow and aggregation.              |
| Federated Learning Iterations    | 11/01/2024 | 11/10/2024 | Conduct multiple rounds of federated training, refining the global model with updates from client devices.              |
| Final Model Tuning    | 11/11/2024 | 11/21/2024 | Optimize the model parameters based on evaluation results and prepare the final model.              |
| Final Review & Submission    | 11/22/2024 | 12/08/2024 | Conduct a final review of the project deliverables, make any necessary revisions, and submit the project.|

## References
1. Multimodal Federated Learning on IOT Data ( https://pure-research.york.ac.uk/ws/portalfiles/portal/79047763/2109.04833v2.pdf)
2. Communication-Efficient learning of deep networks from decentralized data ( http://proceedings.mlr.press/v54/mcmahan17a/mcmahan17a.pdf)
