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
  * **🔧 Method**: ⭐⭐⭐⭐ (4/5) - Investigates how perturbing the visual encoder affects LDM fine-tuning and introduces a lightweight mechanism that disrupts concept learning regardless of the attacker’s prompt.

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

  
<h4 id="Privacy-Preserving 2025"> 2025 </h4>

* **[2024.05.31]** **[PersGuard: Preventing Malicious Personalization via  Backdoor Attacks on Pre-trained Text-to-Image  Diffusion Models](https://openreview.net/forum?id=5WK8ZO2XJW)**
  * Xinwei Liu, Xiaojun Jia, Yuan Xun, Hua Zhang, Xiaochun Cao
  * **📝 Summary**: Prevent malicious personalization of specific images by injecting backdoors into upstream T2I models so protected images fail to produce personalized outputs while unprotected images retain normal personalization.
  * **💡 Motivation**: ⭐⭐⭐⭐ (4/5) - Existing adversarial perturbation defenses for T2I diffusion models lack robustness and cannot fully remove identifiable features.  
  * **🔧 Method**: ⭐⭐⭐ (3/5) - PersGuard injects backdoors into pretrained models with three objectives (Pattern, Erasure, Target), and converts the trigger mechanism into a shortcut such that the backdoor is activated by fine-tuning on a specific image set.

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



