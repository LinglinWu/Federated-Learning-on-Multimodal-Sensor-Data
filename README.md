# Project Title
# Federated-Learning-on-Multimodal-Sensor-Data

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
| Name       | Role               | Responsibilities        |
|------------|---------------------|-------------------------|
| Linglin Wu | Project Setup Lead  | 負責專案初始化與設定    |
| Rui Li     | Software Lead       | 負責軟體開發            |


## Project Timeline
| Milestone  | Start Date | End Date | Description              |
|------------|------------|----------|--------------------------|
| Phase 1    | YYYY-MM-DD | YYYY-MM-DD | 初期研究與規劃          |
| Phase 2    | YYYY-MM-DD | YYYY-MM-DD | 系統設計與開發          |
| Phase 3    | YYYY-MM-DD | YYYY-MM-DD | 測試與驗證              |

## References
1. Multimodal Federated Learning on IOT Data ( https://pure-research.york.ac.uk/ws/portalfiles/portal/79047763/2109.04833v2.pdf)
2.Communication-Efficient learning of deep networks from decentralized data ( http://proceedings.mlr.press/v54/mcmahan17a/mcmahan17a.pdf)
