# CosFairNet: A Parameter-Space based Approach for Bias Free Learning

**Authors:** [Rajeev Ranjan Dwivedi](https://rajeev-dw9.github.io/), Priyadarshini Kumari, Vinod Kumar Kurmi  
**Institution:** Indian Institute of Science Education and Research, Bhopal, India  
**Conference:** BMVC 2024 (Oral)

## Abstract

Deep neural networks trained on biased data often inadvertently learn unintended inference rules, particularly when labels are strongly correlated with biased features. Existing bias mitigation methods typically involve either a) predefining bias types and enforcing them as prior knowledge or b) reweighting training samples to emphasize bias-conflicting samples over bias-aligned samples. However, both strategies address bias indirectly in the feature or sample space, with no control over learned weights, making it difficult to control the bias propagation across different layers. Based on this observation, we introduce a novel approach to address bias directly in the model's parameter space, preventing its propagation across layers. Our method involves training two models: a bias model for biased features and a debias model for unbiased details, guided by the bias model. We enforce dissimilarity in the debias model's later layers and similarity in its initial layers with the bias model, ensuring it learns unbiased low-level features without adopting biased high-level abstractions. By incorporating this explicit constraint during training, our approach shows enhanced classification accuracy and debiasing effectiveness across various synthetic and real-world datasets of different sizes. Moreover, the proposed method demonstrates robustness across different bias types and percentages of biased samples in the training data.

## Resources

- [Paper PDF](static/pdfs/Fairnesss_BMVC_2024.pdf)
- [Supplementary PDF](static/pdfs/CosFairNet_Supplementary.pdf)
- [Code (Coming Soon)](https://visdomlab.github.io/CosFairNet/)

## Model Visualizations

- **Proposed Model Architecture**  
  ![Model Architecture](static/images/1.png)


## Citation

If you find our work useful, please cite it as:

```bibtex
@InProceedings{rajeevbmvc24_abs,
    author    = {Dwivedi, Rajeev R and Kumari, Priyadarshini and Kurmi, Vinod},
    title     = {CosFairNet: A Parameter-Space based Approach for Bias Free Learning},
    booktitle = {Proceedings of the British Machine Vision Conference (BMVC)},
    year      = {2024},
}
