## PMHT：Prompt Feature Fusion with 2DMamba for Hyperspectral Object Tracking

Hyperspectral images offer unique advantages in challenging scenarios such as complex backgrounds, target deformations, and occlusions, thanks to their narrow-band spectral information. However, existing deep learning-based hyperspectral tracking methods are often limited by the scarcity of annotated data, and thus rely on pre-trained RGB trackers, which hinder the full exploitation of spectral features. This results in poor generalization and limited localization accuracy. To address these challenges, this paper proposes a prompt feature fusion with the 2DMamba network (PMHT) for hyperspectral object tracking, leveraging a dual-stream spectral-spatio-temporal prompting mechanism to enhance tracking performance. Specifically, a band selection strategy based on the Neighborhood Group Normalized Matched Filter is designed to select three representative spectral bands as input for the spectral prompt branch. The spatio-temporal prompt is derived from the difference information between consecutive frames. Furthermore, a Prompt Feature Fusion Module is designed in combination with the 2DMamba architecture to effectively integrate the spectral and spatiotemporal prompts with the base features, thereby enhancing the model’s representation of hyperspectral data. Additionally, the loss function is improved through the incorporation of a direction-aware mechanism and a bounding box shape penalty term, which enhances localization accuracy and enforces geometric consistency. Experimental results on the HOTC2024 hyperspectral object tracking dataset demonstrate that the proposed tracker achieves state-of-the-art performance.

###  The flowchart of the proposed algorithm

<img width="5100" height="1958" alt="structure" src="https://github.com/user-attachments/assets/433c0a0a-2607-42a6-91ee-9b273fc317d4" />

### Quantitative performance comparison between PMHT and other SOTA HS trackers on the HOTC2024 dataset

<img width="2795" height="1324" alt="image" src="https://github.com/user-attachments/assets/fb9b5821-6191-4dca-8522-f0522f29bd57" />

### Visualization comparisons of PMHT with other SOTA HS trackers on four video sequences

<img width="2857" height="1296" alt="image" src="https://github.com/user-attachments/assets/f1df3dcb-ebc2-4601-b003-bcff928bdb70" />

