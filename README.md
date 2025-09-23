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

* **[2023.02.09]** **[Adversarial Example Does Good: Preventing Painting Imitation from Diffusion Models via Adversarial Examples](https://openreview.net/forum?id=Wbquvk97t4)** ![Static Badge](https://img.shields.io/badge/ICML'23-dc3545) [![GitHub stars](https://img.shields.io/github/stars/hypknot74/Paper-summaries?style=social)](https://github.com/hypknot74/Paper-summaries)
  * Chumeng Liang, Xiaoyu Wu, Yang Hua, Jiaru Zhang, Yiming Xue, Tao Song, Zhengui XUE, Ruhui Ma, Haibing Guan
  * **📝 Summary**: AdvDM is among the first to tackle this task and reduces the performance (image quality) of diffusion models when using hostile samples in tasks such as T2I and I2I.
  * **💡 Motivation**: ⭐⭐⭐⭐⭐ (5/5) -  Diffusion models enable easy style imitation, yet there are no effective methods to prevent or track such infringements.
  * **🔧 Method**: ⭐⭐⭐ (3/5) - AdvDM creates an adversarial sample by optimizing perturbations to maximize loss by Monte Carlo estimation for various latent variables sampled during the retrodispersion process.

* **[2023.11.22]** **[MetaCloak: Preventing Unauthorized Subject-driven Text-to-image Diffusion-based Synthesis via Meta-learning]([https://openreview.net/forum?id=Wbquvk97t4](https://openaccess.thecvf.com/content/CVPR2024/papers/Liu_MetaCloak_Preventing_Unauthorized_Subject-driven_Text-to-image_Diffusion-based_Synthesis_via_Meta-learning_CVPR_2024_paper.pdf))** ![Static Badge](https://img.shields.io/badge/CVPR'24-dc3545) [![GitHub stars](https://img.shields.io/github/stars/liuyixin-louis/MetaCloak?style=social)](https://github.com/liuyixin-louis/MetaCloak)
  * Yixin Liu, Chenrui Fan, Yutong Dai, Xun Chen, Pan Zhou, Lichao Sun
  * **📝 Summary**: Primarily addresses the transferability and robustness issues of adversarial-based methods targeting personalized generative model.  
  * **💡 Motivation**: ⭐⭐⭐⭐ (4/5) -  Defines existing adversarial-based methods for personalized generation as a bi-level optimization problem, which hand-crafted approaches struggle to handle.  
  * **🔧 Method**: ⭐⭐⭐⭐ (4/5) - Solves the bi-level optimization problem with a meta-learning framework with an additional transformation sampling process to craft transferable and robust perturbation.


<h4 id="Privacy-Preserving 2024"> 2024 </h4>

* **[2024.05.31]** **[Watermark-embedded Adversarial Examples for Copyright Protection against Diffusion Models](https://openaccess.thecvf.com/content/CVPR2024/papers/Zhu_Watermark-embedded_Adversarial_Examples_for_Copyright_Protection_against_Diffusion_Models_CVPR_2024_paper.pdf)** ![Static Badge](https://img.shields.io/badge/CVPR'24-dc3545) 
  * Peifei Zhu, Tsubasa Takahashi, Hirokatsu Kataoka
  * **📝 Summary**: A fast and visible solution for protecting and tracing copyrighted content from imitation by diffusion models.
  * **💡 Motivation**: ⭐⭐⭐⭐⭐ (5/5) - Generates adversarial samples to prevent copyright infringement by diffusion models, forcing them to produce visibly watermarked images for copyright tracking.
  * **🔧 Method**: ⭐⭐⭐ (3/5) - Uses a conditional GAN to train a generator for crafting adversarial examples.

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



