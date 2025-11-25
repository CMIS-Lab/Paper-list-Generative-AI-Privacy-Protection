# 🛡️ Generative AI Privacy Protection Papers Collection

> 📚 **A comprehensive collection of research papers on backdoor defenses in machine learning.**  
> 🎓 **Maintained by**: Dr. [Hu Baoyue] | [Chongqing University of Posts and Telecommunications] | [d230201013@stu.cqupt.edu.cn]

## 📖 About This Repository

<!-- This repository serves as a curated collection of academic papers focusing on **defense mechanisms** in machine learning. Our goal is to provide researchers, practitioners, and students with a comprehensive overview of the current state-of-the-art in this critical security domain. -->
This repository serves as a curated collection of academic papers focusing on **defense mechanisms** for both privacy risks introduced by AIGC applications and security threats to large-scale AIGC models. Our goal is to provide researchers, practitioners, and students with a comprehensive overview of the current state-of-the-art in this critical security domain.



### 🎯 **Repository Purpose:**
- 🏆 **Quality Focus**: Emphasis on high-impact venues. [CCF-Rankings](https://www.ccf.org.cn/en/About_CCF/Media_Center/) now marked with different colors(![arXiv](https://img.shields.io/badge/CCF_A-dc3545) ![Static Badge](https://img.shields.io/badge/CCF_B-ffc107) ![Static Badge](https://img.shields.io/badge/CCF_C-28a745) ![Static Badge](https://img.shields.io/badge/CCF_None-6c757d))
- 🔄 **Regular Updates**: Continuously updated with latest research developments
- 🌐 **Easy Access**: Direct links to papers, code repositories, and supplementary materials

### 📊 **Each paper includes the following evaluation metrics (out of 5 stars):**
- **💡 Motivation**: How well-motivated and significant is the research problem? ⭐⭐⭐⭐⭐ (5/5)
- **🔧 Method**: How novel and technically sound is the proposed approach? ⭐⭐⭐⭐⭐ (5/5)

<h2 id="awesome-papers"> 👑 Awesome Papers List </h2>

<h3 id="Privacy-Preserving"> Privacy-Preserving </h3>

<h4 id="Privacy-Preserving 2023"> 2023 </h4>

* **[2023.03.28]** **[Anti-DreamBooth: Protecting users from personalized text-to-image synthesis](https://openaccess.thecvf.com/content/ICCV2023/papers/Van_Le_Anti-DreamBooth_Protecting_Users_from_Personalized_Text-to-image_Synthesis_ICCV_2023_paper.pdf)** ![Static Badge](https://img.shields.io/badge/ICCV'23-dc3545) [![GitHub stars](https://img.shields.io/github/stars/VinAIResearch/Anti-DreamBooth?style=social)](https://github.com/VinAIResearch/Anti-DreamBooth)
  * Thanh Van Le, Hao Phung, Thuan Hoang Nguyen, Quan Dao, Ngoc N. Tran, Anh Tran
  * **📝 Summary**: Protects images from being exploited by text-to-image models for unauthorized personalization, such as DreamBooth.
  * **💡 Motivation**: ⭐⭐⭐⭐⭐ (5/5) - Text-to-image diffusion models allow anyone to create realistic images from text, but misuse of tools like DreamBooth can generate harmful content targeting individuals.
  * **🔧 Method**: ⭐⭐⭐⭐ (4/5) - Generate adversarial perturbations via Projected Gradient Descent (PGD) to prevent a target model from learning specific image features during DreamBooth fine-tuning.
 
* **[2023.02.09]** **[Adversarial Example Does Good: Preventing Painting Imitation from Diffusion Models via Adversarial Examples](https://openreview.net/forum?id=Wbquvk97t4)** ![Static Badge](https://img.shields.io/badge/ICML'23-dc3545) [![GitHub stars](https://img.shields.io/github/stars/hypknot74/Paper-summaries?style=social)](https://github.com/hypknot74/Paper-summaries)
  * Chumeng Liang, Xiaoyu Wu, Yang Hua, Jiaru Zhang, Yiming Xue, Tao Song, Zhengui XUE, Ruhui Ma, Haibing Guan
  * **📝 Summary**: AdvDM is among the first to prevent diffusion models from imitating images in T2I and I2I tasks using adversarial examples.
  * **💡 Motivation**: ⭐⭐⭐⭐⭐ (5/5) -  Diffusion models enable easy style imitation, yet there are no effective methods to prevent or track such infringements.
  * **🔧 Method**: ⭐⭐⭐ (3/5) - AdvDM creates an adversarial sample by optimizing perturbations to maximize loss by Monte Carlo estimation for various latent variables sampled during the retrodispersion process.

* **[2023.5.22]** **[Mist: Towards improved adversarial examples for diffusion models](https://arxiv.org/abs/2305.12683))**[![GitHub stars](https://img.shields.io/github/stars/psyker-team/mist?style=social)](https://github.com/psyker-team/mist)
  * Chumeng Liang, Xiaoyu Wu
  * **📝 Summary**: Extends AdvDM by improving adversarial losses to generate more transferable and robust adversarial examples against diffusion models imitating paintings.
  * **💡 Motivation**: ⭐⭐ (2/5) - Existing adversarial examples for diffusion models have limited transferability and robustness against simple defenses like noise purification.
  * **🔧 Method**: ⭐⭐⭐ (3/5) - Defines a semantic loss to push image representations away from the model’s semantic space and a texture loss to embed perturbations resembling background watermark patterns.

* **[2023.2.8]** **[Glaze: Protecting Artists from Style Mimicry by Text-to-Image Models](https://www.usenix.org/conference/usenixsecurity23/presentation/shan))** ![Static Badge](https://img.shields.io/badge/usenixsecurity-dc3545) [![GitHub stars](https://img.shields.io/github/stars/EspacioLatente/Glaze?style=social)](https://github.com/EspacioLatente/Glaze)
  * Shawn Shan, Jenna Cryan, Emily Wenger, Haitao Zheng, Rana Hanocka, Ben Y. Zhao
  * **📝 Summary**: Glaze helps artists to prevent their artistic styles from being learned and mimicked by new AI models and their variants.
  * **💡 Motivation**: ⭐⭐⭐⭐ (4/5) - Modern AIGC systems like MidJourney and Stable Diffusion can easily imitate an artist’s style, raising serious concerns over artistic identity and copyright.
  * **🔧 Method**: ⭐⭐ (2/5) - Optimizes feature-level distances between the original and target style representations to induce misleading perturbations, causing diffusion models to learn incorrect artistic styles.

* **[2023.09.21]** **[Diffusion-Based Adversarial Sample Generation for Improved Stealthiness and Controllability](https://proceedings.neurips.cc/paper_files/paper/2023/hash/088463cd3126aef2002ffc69da42ec59-Abstract-Conference.html)** ![Static Badge](https://img.shields.io/badge/NIPS'23-dc3545)  [![GitHub stars](https://img.shields.io/github/stars/xavihart/Diff-PGD?style=social)](https://github.com/xavihart/Diff-PGD)
  * Haotian Xue, Alexandre Araujo, Bin Hu, Yongxin Chen
  * **📝 Summary**: This work presents Diff-PGD, a diffusion-guided adversarial sample generation framework that produces realistic, distribution-aligned perturbations with improved transferability and controllability.
  * **💡 Motivation**: ⭐⭐⭐ (3/5) - The method aims to overcome the inherent trade-off between adversarial strength and visual naturalness in traditional gradient-based attacks, which often produce unrealistic perturbations.
  * **🔧 Method**: ⭐⭐⭐⭐⭐ (5/5) - Diff-PGD leverages diffusion-model-guided gradients to constrain perturbations toward natural image manifolds while decoupling adversarial optimization from auxiliary losses to improve stability and task adaptability.


<h4 id="Privacy-Preserving 2024"> 2024 </h4>

* **[2024.5.31]** **[MetaCloak: Preventing Unauthorized Subject-driven Text-to-image Diffusion-based Synthesis via Meta-learning]([https://openreview.net/forum?id=Wbquvk97t4](https://openaccess.thecvf.com/content/CVPR2024/papers/Liu_MetaCloak_Preventing_Unauthorized_Subject-driven_Text-to-image_Diffusion-based_Synthesis_via_Meta-learning_CVPR_2024_paper.pdf))** ![Static Badge](https://img.shields.io/badge/CVPR'24-dc3545) [![GitHub stars](https://img.shields.io/github/stars/liuyixin-louis/MetaCloak?style=social)](https://github.com/liuyixin-louis/MetaCloak)
  * Yixin Liu, Chenrui Fan, Yutong Dai, Xun Chen, Pan Zhou, Lichao Sun
  * **📝 Summary**: Primarily addresses the transferability and robustness issues of adversarial-based methods targeting personalized generative model.  
  * **💡 Motivation**: ⭐⭐⭐⭐ (4/5) -  Defines existing adversarial-based methods for personalized generation as a bi-level optimization problem, which hand-crafted approaches struggle to handle.  
  * **🔧 Method**: ⭐⭐⭐⭐ (4/5) - Solves the bi-level optimization problem with a meta-learning framework with an additional transformation sampling process to craft transferable and robust perturbation.
  
* **[2024.05.31]** **[Watermark-embedded Adversarial Examples for Copyright Protection against Diffusion Models](https://openaccess.thecvf.com/content/CVPR2024/papers/Zhu_Watermark-embedded_Adversarial_Examples_for_Copyright_Protection_against_Diffusion_Models_CVPR_2024_paper.pdf)** ![Static Badge](https://img.shields.io/badge/CVPR'24-dc3545) 
  * Peifei Zhu, Tsubasa Takahashi, Hirokatsu Kataoka
  * **📝 Summary**: A fast and visible solution for protecting and tracing copyrighted content from imitation by diffusion models.
  * **💡 Motivation**: ⭐⭐⭐⭐ (4/5) - Generates adversarial samples to prevent copyright infringement by diffusion models, forcing them to produce visibly watermarked images for copyright tracking.
  * **🔧 Method**: ⭐⭐ (2/5) - Uses a conditional GAN to train a generator for crafting adversarial examples.

* **[2024.9.28]** **[IMMA: Immunizing text-to-image Models against Malicious Adaptation](https://www.semanticscholar.org/reader/9d967d4a15b55bba08b9f2df85d8e05384f2516c))** ![Static Badge](https://img.shields.io/badge/ECCV'24-ffc107) [![GitHub stars](https://img.shields.io/github/stars/amberyzheng/IMMA?style=social)](https://github.com/amberyzheng/IMMA)
  * Amber Yijia Zheng, Raymond A. Yeh
  * **📝 Summary**: IMMA immunizes text-to-image models so they resist malicious fine-tuning that aims to generate harmful or unauthorized content.
  * **💡 Motivation**: ⭐⭐⭐⭐ (4/5) - Open-source diffusion models can be easily adapted to mimic artists or produce harmful content, yet most existing defenses only poison training data rather than strengthening the model itself.
  * **🔧 Method**: ⭐⭐⭐⭐ (4/5) - Learns model parameters that are inherently difficult for adaptation methods (LoRA, Textual Inversion, DreamBooth) to fine-tune, and applies this before releasing model weights to mitigate malicious personalization.

* **[2024.06.14]** **[PID: Prompt-Independent Data Protection Against Latent Diffusion Models](https://openaccess.thecvf.com/content/C2024/papers/Zhu_Watermark-embedded_Adversarial_Examples_for_Copyright_Protection_against_Diffusion_Models_CVPR_2024_paper.pdf)** ![Static Badge](https://img.shields.io/badge/ICCV'24-dc3545)  [![GitHub stars](https://img.shields.io/github/stars/PKU-ML/Diffusion-PID-Protection?style=social)](https://github.com/PKU-ML/Diffusion-PID-Protection)
  * Ang Li, Yichuan Mo, Mingjie Li, Yisen Wang
  * **📝 Summary**: PID prevents misused few-shot personalization of Latent Diffusion Models by manipulating the visual encoder in a prompt-independent manner.
  * **💡 Motivation**: ⭐⭐⭐⭐ (4/5) - Existing defenses assume protectors and attackers use identical textual prompts, but mismatched conditions significantly reduce their effectiveness; thus a prompt-agnostic defense is needed.
  * **🔧 Method**: ⭐⭐⭐ (3/5) - Investigates how perturbing the visual encoder affects LDM fine-tuning and introduces a lightweight mechanism that disrupts concept learning regardless of the attacker’s prompt.

* **[2024.05.30]** **[Perturbing Attention Gives You More Bang for the Buck: Subtle Imaging Perturbations That Efficiently Fool Customized Diffusion Models](https://openaccess.thecvf.com/content/CVPR2024/papers/Xu_Perturbing_Attention_Gives_You_More_Bang_for_the_Buck_Subtle_CVPR_2024_paper.pdf)** ![Static Badge](https://img.shields.io/badge/CVPR'24-dc3545)  [![GitHub stars](https://img.shields.io/github/stars/CO2-cityao/CAAT?style=social)](https://github.com/CO2-cityao/CAAT)
  * Jingyao Xu, Siyang Lu, Yuetong Lu, Dongdong Wang, Yandong Li, Xiang Wei
  * **📝 Summary**: CAAT exploits the high gradient sensitivity of diffusion cross-attention layers, using tiny perturbations on public images to disrupt personalized text-to-image models.
  * **💡 Motivation**: ⭐⭐⭐ (3/5) - Diffusion models are easily fine-tuned with few images, yet current attacks are either slow or require training; a faster, training-free attack is needed.
  * **🔧 Method**: ⭐⭐⭐⭐ (4/5) - Generates adversarial samples by applying PGD-based perturbations and only modifying the cross-attention keys/values within the U-Net to maximally distort text–image alignment during fine-tuning. 

* **[2024.03.28]** **[Imperceptible Protection against Style Imitation from Diffusion Models](https://arxiv.org/abs/2403.19254)** 
  * Namhyuk Ahn, Wonhyuk Ahn, KiYoon Yoo, Daesik Kim, Seung-Hun Nam
  * **📝 Summary**: This work introduces an imperceptible protection mechanism for text-to-image diffusion models by allocating perturbations based on perceptual sensitivity and difficulty prediction.
  * **💡 Motivation**: ⭐⭐⭐ (3/5) - Existing adversarial protections often degrade visual quality, motivating a more perceptually aligned and high-quality defense.
  * **🔧 Method**: ⭐⭐ (2/5) -The approach applies perceptual maps and instance-wise refinement to allocate perturbations based on visual sensitivity, and predicts protection difficulty to adjust perturbation intensity.

* **[2024.06.16]** **[Toward effective protection against diffusion based mimicry through score distillation](https://proceedings.neurips.cc/paper_files/paper/2023/hash/088463cd3126aef2002ffc69da42ec59-Abstract-Conference.html)** ![Static Badge](https://img.shields.io/badge/ICLR'24-dc3545)  [![GitHub stars](https://img.shields.io/github/stars/xavihart/Diff-Protect?style=social)](https://github.com/xavihart/Diff-Protect)
  * Haotian Xue, Chumeng Liang, Xiaoyu Wu, Yongxin Chen
  * **📝 Summary**: This work reveals that the encoder in latent diffusion models is the primary vulnerability and introduces efficient plug-and-play protection strategies that accelerate perturbation generation while reducing memory cost.
  * **💡 Motivation**: ⭐⭐⭐ (3/5) - The study aims to provide practical and computationally lightweight protection against diffusion-based mimicry attacks, which current defenses struggle to achieve.
  * **🔧 Method**: ⭐⭐⭐ (3/5) - The approach leverages Score Distillation Sampling to optimize perturbations through the encoder pathway and employs a counterintuitive semantic-loss minimization scheme to produce stronger and more natural defensive perturbations.

* **[2024.09.17]** **[Step Vulnerability Guided Mean Fluctuation Adversarial Attack against Conditional Diffusion Models](https://dl.acm.org/doi/abs/10.1609/aaai.v38i7.28503)** ![Static Badge](https://img.shields.io/badge/AAAI'24-dc3545)  [![GitHub stars](https://img.shields.io/github/stars/yuhongwei22/MFA?style=social)](https://github.com/yuhongwei22/MFA)
  * Hongwei Yu, Jiansheng Chen, Xinlong Ding, Yudong Zhang, Ting Tang, Huimin Ma
  * **📝 Summary**: This work exploits diffusion models’ sensitivity to noise-mean shifts and introduces the Mean Fluctuation Attack (MFA), which perturbs the estimated noise means during reverse sampling to destabilize the entire generation process.
  * **💡 Motivation**: ⭐⭐⭐⭐ (4/5) - It aims to reveal and leverage step-wise vulnerability variations in the reverse diffusion process to design more effective adversarial attacks against conditional diffusion models.
  * **🔧 Method**: ⭐⭐⭐⭐ (4/5) - It models step vulnerability to guide sampling of attack-critical timesteps and optimizes perturbations on the conditioning input to maximize the expected mean shift of predicted noise.

* **[2024.01.13]** **[Exploring Adversarial Attacks against Latent Diffusion Model from the Perspective of Adversarial Transferability](https://arxiv.org/abs/2401.07087)**
  * Junxi Chen, Junhao Dong, Xiaohua Xie
  * **📝 Summary**: This work studies how the properties of surrogate models affect adversarial transferability in LDMs and shows that selecting smoother surrogate models enhances the effectiveness of adversarial examples.
  * **💡 Motivation**: ⭐⭐⭐⭐ (4/5) - EExisting approaches suffer from transferability gaps because surrogate models inevitably differ from the target LDMs, reducing the cross-model effectiveness of generated adversarial examples.
  * **🔧 Method**: ⭐⭐ (2/5) - The method treats timestep sampling in Monte Carlo-based adversarial attacks as surrogate model selection and boosts attack success by preferentially sampling timesteps corresponding to smoother surrogate models.

* **[2024.08.20]** **[Prompt-Agnostic Adversarial Perturbation for Customized Diffusion Models](https://proceedings.neurips.cc/paper_files/paper/2024/hash/f6b35e248a21c71ff1cd47b8919fca83-Abstract-Conference.html)** ![Static Badge](https://img.shields.io/badge/NIPS'24-dc3545)  [![GitHub stars](https://img.shields.io/github/stars/vancyland/Prompt-Agnostic-Adversarial-Perturbation-for-Customized-Diffusion-Models?style=social)](https://github.com/vancyland/Prompt-Agnostic-Adversarial-Perturbation-for-Customized-Diffusion-Models.github.io)
  * Cong Wan, Yuhang He, Xiang Song, Yihong Gong
  * **📝 Summary**: This work introduces a prompt-agnostic adversarial perturbation (PAP) method that protects diffusion models from malicious personalization regardless of prompt variations.
  * **💡 Motivation**: ⭐⭐⭐⭐ (4/5) - Existing defenses struggle to generalize because their effectiveness collapses when prompts change, limiting protection in real-world diffusion-based generation.
  * **🔧 Method**: ⭐⭐⭐⭐ (4/5) - PAP models the prompt distribution in the embedding space using a Laplace approximation and generates prompt-agnostic perturbations by maximizing the expected disturbance under this learned distribution.

* **[2024.11.25]** **[Privacy Protection in Personalized Diffusion Models via Targeted Cross-Attention Adversarial Attack](https://arxiv.org/abs/2411.16437)**
  * Xide Xu, Muhammad Atif Butt, Sandesh Kamath, Bogdan Raducanu
  * **📝 Summary**: The method disrupts personalization by forcing a divergence between user-specific and class-specific cross-attention maps during personalized fine-tuning.
  * **💡 Motivation**: ⭐⭐ (2/5) - The work addresses privacy risks in personalized diffusion models by preventing attackers from reconstructing or impersonating an individual’s identity.
  * **🔧 Method**: ⭐⭐ (2/5) - The approach minimizes the cosine similarity between the cross-attention representations of the user-specific token and the class token using a PGD-based perturbation scheme.

  
<h4 id="Privacy-Preserving 2025"> 2025 </h4>

* **[2024.05.31]** **[PersGuard: Preventing Malicious Personalization via  Backdoor Attacks on Pre-trained Text-to-Image  Diffusion Models](https://openreview.net/forum?id=5WK8ZO2XJW)**
  * Xinwei Liu, Xiaojun Jia, Yuan Xun, Hua Zhang, Xiaochun Cao
  * **📝 Summary**: Prevent malicious personalization of specific images by injecting backdoors into upstream T2I models so protected images fail to produce personalized outputs while unprotected images retain normal personalization.
  * **💡 Motivation**: ⭐⭐⭐⭐ (4/5) - Existing adversarial perturbation defenses for T2I diffusion models lack robustness and cannot fully remove identifiable features.  
  * **🔧 Method**: ⭐⭐⭐ (3/5) - PersGuard injects backdoors into pretrained models with three objectives (Pattern, Erasure, Target), and converts the trigger mechanism into a shortcut such that the backdoor is activated by fine-tuning on a specific image set.

* **[2025.05.15]** **[Towards Reliable Verification of Unauthorized Data Usage in Personalized Text-to-Image Diffusion Models](https://ieeexplore.ieee.org/abstract/document/11023473)** ![Static Badge](https://img.shields.io/badge/S&P'25-dc3545)  [![GitHub stars](https://img.shields.io/github/stars/AntigoneRandy/SIREN?style=social)](https://github.com/AntigoneRandy/SIREN)
  * Boheng Li; Yanhao Wei; Yankai Fu; Zhenting Wang; Yiming Li; Jie Zhang
  * **📝 Summary**: The key contribution of this work is a verifiable coating (perturbation) mechanism that reliably reveals unauthorized data usage in personalized diffusion models.
  * **💡 Motivation**: ⭐⭐⭐⭐ (4/5) - Existing coating-based traceability methods fail in personalization because the coatings are not learned as meaningful features, making verification weak and unreliable.
  * **🔧 Method**: ⭐⭐⭐ (3/5) - SIREN optimizes coatings to align with personalization-relevant features and incorporates perceptual constraints, hypersphere classification, and hypothesis-testing–guided verification to boost stealthiness and detection accuracy.
 
* **[2025.02.12]** **[ID-Cloak: Crafting Identity-Specific Cloaks Against Personalized Text-to-Image Generation](https://arxiv.org/abs/2502.08097)** [![GitHub stars](https://img.shields.io/github/stars/ID-Cloak/ID-Cloak?style=social)](https://github.com/ID-Cloak/ID-Cloak/blob/main/README.md)
  * Qianrui Teng, Xing Cui, Xuannan Liu, Peipei Li, Zekun Li, Huaibo Huang, Ran He
  * **📝 Summary**:The work constructs a universal, identity-level cloak that protects all images of the same person by perturbing them within a learned identity subspace.
  * **💡 Motivation**: ⭐⭐⭐⭐ (4/5) - The goal is to overcome the impracticality of image-specific cloaking by enabling scalable privacy protection against personalized T2I models.
  * **🔧 Method**: ⭐⭐⭐⭐ (4/5) - The approach models an identity semantic subspace in text-embedding space and optimizes a universal perturbation via PGD+SGA to steer generated outputs away from the protected identity.

* **[2025.01.22]** **[Protecting your portraits: Real-time Identity Defense against malicious personalization of diffusion models](https://arxiv.org/html/2412.09844v2)** [![GitHub stars](https://img.shields.io/github/stars/Guohanzhong/RID?style=social)](https://github.com/Guohanzhong/RID)
  * Hanzhong Guo, Shen Nie, Chao Du, Tianyu Pang, Hao Sun, Chongxuan Li
  * **📝 Summary**: This work introduces RID, a real-time network that produces adversarial perturbations via a single forward pass, enabling highly efficient and robust identity protection against malicious personalization.
  * **💡 Motivation**: ⭐⭐⭐ (3/5) - It aims to overcome the impracticality of optimization-based defenses by developing a fast, deployable, and model-agnostic protection mechanism.
  * **🔧 Method**: ⭐⭐⭐⭐⭐ (5/5) - RID directly predicts perturbations through an end-to-end network and enhances cross-model and post-processing robustness using an ensemble of diffusion models, eliminating the need for costly per-image optimization.
 
* **[2025.02.28]** **[Latent Diffusion Shield - Mitigating Malicious Use of Diffusion Models Through Latent Space Adversarial Perturbations](https://openaccess.thecvf.com/content/WACV2025W/SynRDinBAS/papers/Phan_Latent_Diffusion_Shield_-_Mitigating_Malicious_Use_of_Diffusion_Models_WACVW_2025_paper.pdf)** ![Static Badge](https://img.shields.io/badge/WACV'25-6c757d)  
  * Huy Phan; Boshi Huang; Ayush Jaiswal; Ekraam Sabir; Prateek Singhal; Bo Yuan
  * **📝 Summary**: Proposes a latent-space adversarial protection mechanism that prevents unauthorized diffusion-based image synthesis while keep lightweight.
  * **💡 Motivation**: ⭐⭐⭐ (3/5) - Highlights the urgent need for a generalized, lightweight, and real-time defense against malicious personalization and copyright misuse in diffusion models.
  * **🔧 Method**: ⭐⭐ (2/5) - Offers two variants, an iterative plug-and-play version (LDS-I) and a real-time generative version (LDS-RT), which jointly disrupt both the encoder and U-Net denoising process by optimizing latent-level adversarial noise.

* **[2025.07.21]** **[IDProtector: An Adversarial Noise Encoder to Protect Against ID-Preserving Image Generation](https://openaccess.thecvf.com/content/CVPR2025/html/Song_IDProtector_An_Adversarial_Noise_Encoder_to_Protect_Against_ID-Preserving_Image_CVPR_2025_paper.html)** ![Static Badge](https://img.shields.io/badge/CVPR'25-dc3545) [![GitHub stars](https://img.shields.io/github/stars/yangpei-comp/IDProtector_Preview?style=social)](https://github.com/yangpei-comp/IDProtector_Preview)
  * Yiren Song, Pei Yang, Hai Ci, Mike Zheng Shou
  * **📝 Summary**: Provides a universal protection mechanism against encoder-based identity-preserving generation methods—including InstantID, IP-Adapter, and PhotoMaker—by applying imperceptible adversarial noise to portrait images.
  * **💡 Motivation**: ⭐⭐⭐ (3/5) - Addresses the emerging privacy risks brought by zero-shot identity-preserving generation methods, which enable instant personalization from a single portrait.
  * **🔧 Method**: ⭐⭐ (2/5) - Introduces an adversarial noise encoder that generates perturbations in a single forward pass, offering robust and generalizable protection across multiple diffusion models and image transformations, without requiring image-specific optimization.

* **[2025.05.19]** **[Harnessing Global-local Collaborative Adversarial Perturbation for Anti-Customization](https://openaccess.thecvf.com/content/CVPR2025/papers/Xu_Harnessing_Global-Local_Collaborative_Adversarial_Perturbation_for_Anti-Customization_CVPR_2025_paper.pdf)** ![Static Badge](https://img.shields.io/badge/CVPR'25-dc3545) [![GitHub stars](https://img.shields.io/github/stars/xl-yaoyi/GoodAC?style=social)](https://github.com/xl-yaoyi/GoodAC)
  * Long Xu, Jiakai Wang, Haojie Hao, Haotong Qin, Jiejie Zhao, Xianglong Liu
  * **📝 Summary**: Proposes GoodAC, a global–local collaborative adversarial framework that enhances anti-customization robustness by simultaneously disrupting global feature correlations and local personalized facial attributes.
  * **💡 Motivation**: ⭐⭐⭐⭐ (4/5) - Existing adversarial anti-customization methods overlook hierarchical characteristics, resulting in weak defense against concept transfer and semantic stealing.
  * **🔧 Method**: ⭐⭐⭐⭐ (4/5) - Introduces a two-branch strategy: globally breaking spatial correlations in perceptual features to resist concept transfer, and locally distorting identity-specific facial attributes to prevent semantic extraction.

* **[2025.06.02]** **[Adv-CPG: A Customized Portrait Generation Framework with Facial Adversarial Attacks](https://openaccess.thecvf.com/content/CVPR2025/papers/Wang_Adv-CPG_A_Customized_Portrait_Generation_Framework_with_Facial_Adversarial_Attacks_CVPR_2025_paper.pdf)** ![Static Badge](https://img.shields.io/badge/CVPR'25-dc3545) [![GitHub stars](https://img.shields.io/github/stars/JunyingWang959/Adv-CPG?style=social)](https://github.com/JunyingWang959/Adv-CPG)
  *  Junying Wang, Hongyuan Zhang, Yuan Yuan
  * **📝 Summary**: The first customized portrait generation framework Adv-CPG that embeds facial adversarial attacks to protect identities while enabling fine-grained, controllable portrait synthesis.
  * **💡 Motivation**: ⭐⭐⭐⭐⭐ (5/5) - Existing customized portrait generation methods produce realistic results but fail to prevent generated portraits from being tracked or misused by face recognition systems.
  * **🔧 Method**: ⭐⭐⭐⭐ (4/5) - Designs a two-stage adversarial identity encryption pipeline consisting of a lightweight local ID encryptor and an encryption enhancer for progressive protection, combined with a multimodal customizer that generates precise, fine-grained facial features under adversarial constraints.

   
 
<h3 id="Privacy-Violating"> Privacy-Violating </h3>
<h4 id="Privacy-Violating 2024"> 2024 </h4>

* **[2024.06.21]** **[EvilEdit: Backdooring Text-to-Image Diffusion Models in One Second](https://openreview.net/forum?id=ibEaSS6bQn)** ![Static Badge](https://img.shields.io/badge/ACMMM'24-dc3545) [![GitHub stars](https://img.shields.io/github/stars/haowang02/EvilEdit?style=social)](https://github.com/haowang02/EvilEdit)
  * Hao Wang, Shangwei Guo, Jialing He, Kangjie Chen, Shudong Zhang, Tianwei Zhang, Tao Xiang
  * **📝 Summary**: Backdoor insertion for text-to-image diffusion models is achieved in a training-free and data-free manner by adopting a lightweight model editing approach.
  * **💡 Motivation**: ⭐⭐⭐⭐ (4/5) - A closed-form global minimizer of backdoor model weights derived from the loss function removes the reliance on poisoned datasets and fine-tuning.
  * **🔧 Method**: ⭐⭐⭐ (3/5) - Projection matrices in the cross-attention layers of the diffusion model are directly edited to align the trigger with its corresponding backdoor target.
 
 <h4 id="Privacy-Violating 2025"> 2025 </h4>
 
 * **[2025.03.13]** **[Silent Branding Attack Trigger-free Data Poisoning Attack on Text-to-Image Diffusion](https://openaccess.thecvf.com/content/CVPR2025/papers/Jang_Silent_Branding_Attack_Trigger-free_Data_Poisoning_Attack_on_Text-to-Image_Diffusion_CVPR_2025_paper.pdf)** ![Static Badge](https://img.shields.io/badge/CVPR'25-dc3545) [![GitHub stars](https://img.shields.io/github/stars/agwmon/silent-branding-attack?style=social)](https://github.com/agwmon/silent-branding-attack)
   * Sangwon Jang, June Suk Choi, Jaehyeong Jo, Kimin Lee, Sung Ju Hwang
   * **📝 Summary**: Proposes a data poisoning method that injects logos into training images so that diffusion models generate them naturally without text triggers.  
   * **💡 Motivation**: ⭐⭐⭐ (3/5) - Repeated visual patterns in training data lead models to reproduce them in outputs even without explicit prompts.  
   * **🔧 Method**: ⭐⭐⭐⭐ (4/5) - Finetune SDXL on few-shot logo exemplars, locate natural insertion regions via iterative SDEdit and Detect-and-Compare (OWL-v2 + DINOv2 with augmented references), then paste, style-aligned inpaint, and zoom-refine until detection succeeds.



