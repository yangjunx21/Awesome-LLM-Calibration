# Awesome LLM Calibration

A curated list of papers, toolkits, and other resources for Large Language Model (LLM) Calibration (Confidence, Uncertainty Quantification and so on). 🧠

Welcome to share your papers, thoughts and ideas in this area! 💪 💪 💪 

## Contents

  - [Surveys and Tutorials](#Surveys-and-Tutorials)
  - [Highlight Papers](#Highlight-Papers)
  - [Paper Collections](#Paper-Collections)
  - [Toolkits & Libraries](#Toolkits-Libraries)
  - [Contributing](#Contributing)

-----

## Surveys and Tutorials

*Broad overviews of the calibration and uncertainty quantification landscape.*

  - **Uncertainty Quantification for Large Language Models**
      - Artem Shelmanov，Maxim Panov，Roman Vashurin, et al. 
      - `ACL 2025 Tutorial`
      - [link](https://sites.google.com/view/acl2025-uncertainty-for-llms/)

  - **A Survey of Confidence Estimation and Calibration in Large Language Models**

      - *Zheng Geng, Renjie Pi, Yifei Li, et al. (Tsinghua University, 2024)*
      - `NAACL 2024`
      - [[Paper]](https://aclanthology.org/2024.naacl-long.366/)

  - **Uncertainty Quantification and Confidence Calibration in Large Language Models: A Survey**

      - *Jia-Chen Liu, Zhen-Hui Liu, Yuming-Zhang, et al. (Beijing University of Posts and Telecommunications, 2024)*
      - `arXiv 2024`
      - [[Paper]](https://arxiv.org/abs/2402.13419)

  - **Uncertainty Estimation for Natural Language Processing (Tutorial)**

      - *Chrysoula Zerva, André F. T. Martins, et al. (Unbabel, Instituto de Telecomunicações)*
      - `COLING 2022`
      - [[Website]](https://sites.google.com/view/uncertainty-nlp)

  - **A Survey on Uncertainty Quantification in Deep Learning**

      - *Jie-Fang Zhang, Chen-Xiao-Ma, et al. (Beihang University, 2023)*
      - `arXiv 2023`
      - [[Paper]](https://arxiv.org/abs/2302.09520)

  - **Conformal Prediction for Natural Language Processing: A Survey**

      - *Robert L. Logan IV, AndreaASF, et al. (UMass Amherst, 2024)*
      - `TACL 2024`
      - [[Paper]](https://arxiv.org/abs/2309.02758)


-----

## Highlight Papers

Seminal and impactful papers from renowned labs like OpenAI / Anthropic / ... and conferences (Spotlight/Oral presentations or higher).

  - **Language Models (Mostly) Know What They Know**

      - *Saurav Kadavath, Tom Conerly, Amanda Askell, et al. (Anthropic, 2022)*
      - `arXiv 2022`
      - [[Paper]](https://arxiv.org/abs/2207.05221)

  - **Teaching Models to Express Their Uncertainty in Words**

      - *Stephanie Lin, Jacob Hilton, Owain Evans (OpenAI, 2022)*
      - `OpenAI Blog`
      - [[Post]](https://openai.com/index/teaching-models-to-express-their-uncertainty-in-words/)

  - **Calibrating Large Language Models Using Their Generations**

      - *Theodore Z. Zhao, Moin Nadeem, Sanjiv Kumar, Himabindu Lakkaraju (Harvard & Google, 2024)*
      - `ICLR 2024`
      - [[Paper]](https://arxiv.org/abs/2310.05499)

  - **Pretraining Data Detection for Large Language Models: A Divergence-based Calibration Method**

      - *Se-Eun Yoon, Ji-Hoon Kim, Jae-Hoon Kim, Jae-Min Kim (KAIST AI, 2024)*
      - `EMNLP 2024 (Best Paper)`
      - [[Paper]](https://arxiv.org/abs/2405.08331)

-----

## Paper Collections

### Confidence & Uncertainty Estimation Methods

#### White-Box Methods (Logit/Internal State-based)

*Methods that require access to model internals like logits, probabilities, or hidden states.*

  - **Semantic Uncertainty: Linguistic Invariances for Uncertainty Estimation in Natural Language Generation**

      - *Lorenz Kuhn, Yarin Gal, Sebastian Farquhar (University of Oxford, 2023)*
      - `ICML 2023`
      - [[Paper]](https://arxiv.org/abs/2202.09673)

  - **The Internal State of an LLM Knows When It’s Lying**

      - *Amos Azaria, Tom Mitchell (Carnegie Mellon University, 2023)*
      - `arXiv 2023`
      - [[Paper]](https://arxiv.org/abs/2304.13734)

  - **DoLa: Decoding by Contrasting Layers to Prevent Hallucinations**

      - *K. K. Chuang, X. Li, H. Li, J. D. D. Gross, R. R. R. Manavalan, Y. Tian, H. W. Lee, H. Lee, A. Torralba, S. W. Lee (MIT, 2023)*
      - `arXiv 2023`
      - [[Paper]](https://arxiv.org/abs/2309.03883)

#### Black-Box Methods (Generation-based)

*Methods that estimate uncertainty using only the model's generated text outputs.*

  - **SelfCheckGPT: Zero-Resource Black-Box Hallucination Detection for Generative Large Language Models**

      - *Potsawee Manakul, Adian Liusie, Mark J. F. Gales (University of Cambridge, 2023)*
      - `EMNLP 2023`
      - [[Paper]](https://arxiv.org/abs/2303.08896)

  - **Generating with Confidence: Uncertainty Quantification for Black-box Large Language Models**

      - *Itay Itzhak, Si-An Chen, Li-Wei Chen, et al. (Tel Aviv University, 2023)*
      - `arXiv 2023`
      - [[Paper]](https://arxiv.org/abs/2305.19187)

  - **Strength in Numbers: Estimating Confidence of Large Language Models by Prompt Agreement**

      - *Roi Cohen, Elad Venezian, Mor Geva (Tel Aviv University & Google, 2024)*
      - `NAACL 2024`
      - [[Paper]](https://arxiv.org/abs/2312.01026)

### Calibration Methods

#### Post-Hoc Calibration Methods

*Techniques applied after model training to rescale confidence scores.*

  - **How Can We Know When Language Models Know? On the Calibration of Language Models for Question Answering**

      - *Zhengbao Jiang, Junru Lu, et al. (Carnegie Mellon University, 2021)*
      - `RepL4NLP 2021`
      - [[Paper]](https://arxiv.org/abs/2012.00955)

  - **Few-Shot Recalibration of Language Models**

      - *Zhizheng Zhang, Shuo Chen, Gyorgy Tur, et al. (Google Research, 2024)*
      - `NAACL 2024`
      - [[Paper]](https://aclanthology.org/2024.naacl-long.446/)

#### Intrinsic & Training-Time Methods

*Methods integrated into the model's training process to improve calibration.*

  - **Mix-n-Match: Ensemble and Compositional Methods for Uncertainty Calibration in Long-form Question Answering**

      - *J. M. He, M. Q. Lam, R. Z. Tan, D. M. Blei, A. G. Wilson (NYU, 2022)*
      - `ICML 2022`
      - [[Paper]](https://arxiv.org/abs/2205.13217)

  - **Calibrating Multimodal Learning**

      - *S. Letellier, Y. Feng, R. K. Gupta, J. Z. Liu, P. H. S. Torr (University of Oxford, 2023)*
      - `ICML 2023 (Oral)`
      - [[Paper]](https://www.google.com/search?q=https://arxiv.org/abs/2306.11871)

### Specialized Techniques

#### Bayesian & Ensemble Approaches

  - **Packed-Ensembles for Efficient Uncertainty Estimation**

      - *Z. Wen, J. D. K. Fellow, S. Shrestha, S. Khan, F. S. Khan, T. M. Hospedales (MBZUAI & University of Edinburgh, 2023)*
      - `ICLR 2023 (Oral)`
      - [[Paper]](https://arxiv.org/abs/2211.13328)

#### Conformal Prediction

  - **Conformal Prediction: A Gentle Introduction**

      - *Anastasios N. Angelopoulos, Stephen Bates (UC Berkeley & Carnegie Mellon University)*
      - `Foundations and Trends® in Machine Learning, 2023`
      - [[Paper]](https://arxiv.org/abs/2107.07511)

  - **Conformalized Language Models**

      - *Z. Ren, J. Z. Liu, Y. Gal, B. van der Schaar (University of Cambridge, 2023)*
      - `arXiv 2023`
      - [[Paper]](https://arxiv.org/abs/2307.04212)

-----

## Toolkits & Libraries

*Open-source libraries to help you measure and improve model calibration.*

  - **LM-Polygraph**

      - **Link:** [`https://github.com/IINemo/lm-polygraph`](https://github.com/IINemo/lm-polygraph)
      - **Description:** A framework for comparing and evaluating uncertainty estimation methods for large language models.

  - **Uncertainty Toolbox**

      - **Link:** [`https://github.com/uncertainty-toolbox/uncertainty-toolbox`](https://github.com/uncertainty-toolbox/uncertainty-toolbox)
      - **Description:** A Python toolbox for predictive uncertainty quantification, calibration, and visualization.

  - **uqlm**

      - **Link:** [`https://github.com/cvs-health/uqlm`](https://github.com/cvs-health/uqlm)
      - **Description:** A Python library for uncertainty quantification in language models, supporting methods like MC-dropout and ensembles.

  - **uncertainty-calibration**

      - **Link:** [`https://pypi.org/project/uncertainty-calibration/`](https://pypi.org/project/uncertainty-calibration/)
      - **Description:** A library for measuring and performing calibration of uncertainty estimates for regression tasks.

  - **calibration-tuning**

      - **Link:** [`https://github.com/activatedgeek/calibration-tuning`](https://github.com/activatedgeek/calibration-tuning)
      - **Description:** Code for the paper "Fine-tuning Ensembles for Uncertainty Estimation".

-----

## Contributing

Your contributions are always welcome\! If you have any suggestions for adding or removing projects, feel free to open an issue or pull request.

Let's make LLMs more reliable together\! 💪
