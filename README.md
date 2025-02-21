## Group Action Recognition Using Hybrid CNN-LSTM and CNN-ViT Models

### Overview
Group Action Recognition is the task of classifying collective activities by analyzing interactions among individuals in a scene. Unlike individual action recognition, it requires capturing spatial-temporal relationships among multiple subjects. This project implements two hybrid deep learning architectures, **CNN-LSTM** and **CNN-ViT**, to enhance the recognition of group actions by effectively capturing spatial and temporal dependencies.

### Methodology
- **CNN + LSTM Model**
  - CNN extracts spatial features from video frames.
  - LSTM captures temporal dependencies, enabling the model to understand sequential relationships in group activities.

- **CNN + Vision Transformer (ViT) Model**
  - CNN extracts spatial features.
  - ViT leverages self-attention mechanisms to model long-range dependencies and enhance the understanding of group interactions.

### Dataset
We use the **Collective Activity Dataset** [1], which includes video sequences labeled with different group activities such as talking, queuing, dancing, and jogging. The **walking** class is removed as it does not represent a collective activity.


### Results
The models are evaluated on the Collective Activity Dataset, and results demonstrate improvements in group action recognition using hybrid architectures. Below is an example of correctly classified activities:

![Sample Predictions](images/sample_predictions.png)

### References
1. Wongun Choi, K. Shahid, and S. Savarese, "What are they doing? : Collective activity classification using spatio-temporal relationship among people," *2009 IEEE 12th International Conference on Computer Vision Workshops (ICCVW)*, 2009.


