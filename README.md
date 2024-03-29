# Causality Guided Disentanglement for Cross-Platform Hate Speech Detection

![Screenshot](arch.pdf)


Despite their value in promoting open discourse, social media platforms are often exploited to spread harmful content. Current deep learning and natural language processing models used for detecting this harmful content overly rely on domain-specific terms affecting their capabilities to adapt to generalizable hate speech detection. This is because they tend to focus too narrowly on particular linguistic signals or the use of certain categories of words. Another significant challenge arises when platforms lack high-quality annotated data for training, leading to a need for cross-platform models that can adapt to different distribution shifts. Our research introduces a cross-platform hate speech detection model capable of being trained on one platform's data and generalizing to multiple unseen platforms.  To achieve good generalizability across platforms, one way is to disentangle the input representations into invariant and platform-dependent features. We also argue that learning causal relationships, which remain constant across diverse environments, can significantly aid in understanding invariant representations in hate speech. By disentangling input into platform-dependent features (useful for predicting hate targets) and platform-independent features (used to predict the presence of hate), we learn invariant representations resistant to distribution shifts. These features are then used to predict hate speech across unseen platforms. Our extensive experiments across four platforms highlight our model's enhanced efficacy compared to existing state-of-the-art methods in detecting generalized hate speech.

**NOTE**: Current implementation uses FineTuned Roberta and BART encoders and decoders respectively. You can finetune based on your dataset or if you need the finetuned versions used in our model kindly reach out to me at [psheth5@asu.edu](mailto:psheth5@asu.edu) and I can share the google drive for the datasets and the finetuned models.

If you use our code, please cite our work:

```bibtex
@article{sheth2023causality,
  title={Causality Guided Disentanglement for Cross-Platform Hate Speech Detection},
  author={Sheth, Paras and Kumarage, Tharindu and Moraffah, Raha and Chadha, Aman and Liu, Huan},
  journal={arXiv preprint arXiv:2308.02080},
  year={2023}
}
