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

<h3 id="privacy defense"> Privacy Defenses in Generative AI </h3>

<h4 id="privacy defense 2023"> 2023 </h4>

* **[2023.02.09]** **[Adversarial Example Does Good: Preventing Painting Imitation from Diffusion Models via Adversarial Examples](https://openreview.net/forum?id=Wbquvk97t4)** ![Static Badge](https://img.shields.io/badge/ICML'23-6c757d) [![GitHub stars](https://img.shields.io/github/stars/hypknot74/Paper-summaries?style=social)](https://github.com/hypknot74/Paper-summaries)
  * Chumeng Liang, Xiaoyu Wu, Yang Hua, Jiaru Zhang, Yiming Xue, Tao Song, Zhengui XUE, Ruhui Ma, Haibing Guan
  * **📝 Summary**: AdvDM is among the first to tackle this task and reduces the performance (image quality) of diffusion models when using hostile samples in tasks such as T2I and I2I.
  * **💡 Motivation**: ⭐⭐⭐⭐⭐ (5/5) -  Diffusion models enable easy style imitation, yet there are no effective methods to prevent or track such infringements.
  * **🔧 Method**: ⭐⭐⭐ (3/5) - AdvDM creates an adversarial sample by optimizing perturbations to maximize loss by Monte Carlo estimation for various latent variables sampled during the retrodispersion process.

* **[2023.11.22]** **[MetaCloak: Preventing Unauthorized Subject-driven Text-to-image Diffusion-based Synthesis via Meta-learning]([https://openreview.net/forum?id=Wbquvk97t4](https://openaccess.thecvf.com/content/CVPR2024/papers/Liu_MetaCloak_Preventing_Unauthorized_Subject-driven_Text-to-image_Diffusion-based_Synthesis_via_Meta-learning_CVPR_2024_paper.pdf))** ![Static Badge](https://img.shields.io/badge/CVPR'24-6c757d) [![GitHub stars](https://img.shields.io/github/stars/liuyixin-louis/MetaCloak?style=social)](https://github.com/liuyixin-louis/MetaCloak)
 * Yixin Liu; Chenrui Fan; Yutong Dai; Xun Chen; Pan Zhou; Lichao Sun
  * **📝 Summary**: Primarily addresses the transferability and robustness issues of adversarial-based methods targeting personalized generative model.  
  * **💡 Motivation**: ⭐⭐⭐⭐⭐ (4/5) -  Defines existing adversarial-based methods for personalized generation as a bi-level optimization problem, which hand-crafted approaches struggle to handle.  
  * **🔧 Method**: ⭐⭐⭐ (3/5) - Solves the bi-level optimization problem with a meta-learning framework with an additional transformation sampling process to craft transferable and robust perturbation.


<h4 id="privacy defense 2024"> 2024 </h4>

<h4 id="privacy defense 2025"> 2025 </h4>
