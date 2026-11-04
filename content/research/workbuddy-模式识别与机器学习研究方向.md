# 模式识别与机器学习研究方向

> 基于 Prof. Yi Wang（王艺）研究团队成果整理 | 东莞理工学院 · 计算机科学与技术学院

---

## 语言切换 / Language Switch

> 点击下方折叠区域展开对应语言版本。
> Click the sections below to expand the language version you need.

| 中文版 | English Version |
|:---:|:---:|
| 👇 展开下方中文版 | 👇 Expand English version below |

---

<details>
<summary><b>🇨🇳 中文版（点击展开）</b></summary>

# 模式识别与机器学习：从对抗样本到生成式数据增强

## 一、研究方向概述

现代深度学习系统已成为计算机视觉、生物特征安全、医学影像和协同计算等领域的关键基础设施。然而，深度学习模型仍然面临**对抗攻击、隐私泄露和数据分布偏移**等严峻挑战。

本研究方向聚焦**模式识别与机器学习**，贯穿**对抗机器学习（AML）**与**生成式数据增强**两大主线，通过理解模型脆弱性来构建安全、鲁棒、隐私保护和计算高效的机器学习模型。

## 二、三大研究板块

```
                    研究范畴
                       │
     ┌─────────────────┼─────────────────┐
     │                 │                 │
  1.对抗机器学习    2.协同训练与蒸馏    3.生成模型与数据增强
     │                 │                 │
  · 攻击与防御       · 联邦学习         · 数据蒸馏
  · 检测与鲁棒性     · 知识蒸馏         · PEFT与合成
```

---

### 板块一：对抗机器学习——攻击、防御与鲁棒性

研究模型在开放环境下的静态与动态威胁，兼顾模型效用与安全性。

| 研究方向 | 核心成果 |
|:---|:---|
| **高效查询对抗攻击** | 提出 **DAIR** 算法，针对CBIR图像检索系统的决策型黑盒攻击，系统查询开销降低 **87%**，成功绕过微软必应等商业检索引擎（ACM SIGIR 2021） |
| **模型无关对抗检测** | 通过对输入空间施加随机扰动，利用输出统计变化模式检测低幅度对抗噪声 |
| **集成特征鲁棒增强** | 提出 **PDD** 与 **DEG** 方法，通过多视角基网络特征多样化优化集成模型对抗鲁棒性（AAAI 2021） |

---

### 板块二：协同训练、联邦学习与知识蒸馏

解决非独立同分布（长尾）数据、客户端异构性、隐私泄露与通信瓶颈问题。

| 研究方向 | 核心成果 |
|:---|:---|
| **长尾异构联邦学习** | **FedHyb / FedDDL** 框架：客户端实例采样 + 服务器类别均衡代理数据集蒸馏，解决分类器偏差，在极端非独立同分布（α=0.5, IF=100）下表现优异（ECAI 2024） |
| **自适应对抗蒸馏** | **AdaAD**：在对抗博弈框架下优化小容量学生模型训练，动态搜索对齐锚点，同时提升精度与鲁棒性（CVPR 2023） |
| **隐私推断与泄露审计** | 揭示协同学习中深度特征空间的属性推断、样本重构和成员推断漏洞（IEEE ICME 2022） |
| **单轮通信联邦学习** | **SEDAG** 框架：基于无数据多专家蒸馏实现单轮服务器聚合，降低通信成本与中毒攻击风险 |

---

### 板块三：生成模型、数据增强与模型微调

利用 GAN、扩散模型和自回归 Transformer 解决数据稀缺、领域偏移和隐私约束。

| 研究方向 | 核心成果 |
|:---|:---|
| **鲁棒特征适配器（RFA）** | 即插即用适配器，训练中动态生成对抗扰动。ViT对抗训练加速 **>4倍**，参数开销降至 **<1/10**，鲁棒性增益 **>50%**（ECAI 2025） |
| **影响引导扩散（IGD）** | 在反向扩散采样中引入目标梯度引导，免训练生成任务自适应代理数据集（ICLR 2025） |
| **扩散重建数据似然估计** | 通过DDPM部分重建偏差量化数据似然度，用于核心集选择，支持增量学习与边缘部署（AAAI 2026） |
| **跨模态医学图像融合** | **FedMCA**：基于交叉注意力的个性化多模态联邦学习，解决模态异构MRI分割与分类（ICMSSP 2026） |
| **超材料逆向设计** | 3D条件扩散模型 + 拓扑导数数据增强，合成指定弹性模量与电导率的超材料几何结构 |

---

## 三、核心思想：从对抗样本到生成式数据增强

```
  对抗样本                          数据增强
    │                                 │
    ├── 学习数据空间的有效扰动 ────────┤
    │                                 │
    ├── 利用高维空间"线性敏感性" ──────┤
    │                                 │
    └── 提升模型鲁棒性与泛化能力 ──────┘
```

| 维度 | 对抗样本 | 数据增强 |
|:---|:---|:---|
| **扰动目标** | 约束条件下定向扰动，目标是"破坏模型性能" | 分布约束下自然扰动，目标是"保持语义、增加变化" |
| **扰动方式** | 定向累积扰动实现错误分类 | 微小扰动不改变语义，仅增加多样性 |
| **核心价值** | 通过对抗训练暴露脆弱点，学会应对安全威胁 | 补充训练数据覆盖更多场景，缓解数据稀缺与分布偏移 |

> **核心观点：** 模型能力上限取决于数据质量、结构与组织方式。

---

## 四、代表性论文

| 年份 | 论文标题 | 发表 venue | 主题 |
|:---|:---|:---|:---|
| 2026 | Diffusion Reconstruction-Based Data Likelihood Estimation for Core-Set Selection | **AAAI 2026** | 数据蒸馏/扩散模型 |
| 2026 | FedMCA: Cross-Attention-Based Personalized Multimodal Federated Learning | **ICMSSP 2026** | 多模态医学联邦学习 |
| 2025 | Robustness Feature Adapter for Efficient Adversarial Training | **ECAI 2025** | 高效对抗训练/PEFT |
| 2025 | Influence-Guided Diffusion for Dataset Distillation | **ICLR 2025** | 生成式数据集蒸馏 |
| 2025 | StableGuard: Towards Unified Copyright Protection and Tamper Localisation | **NeurIPS 2025** | AI安全与水印 |
| 2024 | Federated Learning with Hybrid Knowledge Distillations on Long-Tailed Data | **ECAI 2024** | 长尾联邦学习 |
| 2023 | Boosting Accuracy and Robustness via Adaptive Adversarial Distillation | **CVPR 2023** | 对抗知识蒸馏 |
| 2022 | Individual Property Inference Over Collaborative Learning | **IEEE ICME 2022** | 联邦学习隐私泄露 |
| 2021 | DAIR: A Query-Efficient Decision-Based Attack On Image Retrieval | **ACM SIGIR 2021** | 黑盒CBIR攻击 |
| 2021 | Adversarial Defence By Diversified Simultaneous Training Of Deep Ensembles | **AAAI 2021** | 深度集成鲁棒性 |

---

## 五、科研项目与知识产权

- **国家自然科学基金面上项目**：对抗环境下生物特征识别与检索的隐私安全问题研究（Grant No. 61876040，直接经费65万元）
- **广东省基础与应用基础研究基金联合项目**：边缘端生命体征信号智能处理（与中山大学联合申报）
- **专利**：持有多项美国及中国发明专利，涵盖对抗检测、安全哈希检索、隐私保护联邦训练

---

## 六、联系方式

- **单位：** 东莞理工学院计算机科学与技术学院（松山湖校区）
- **邮箱：** wangyi@dgut.edu.cn

</details>

---

<details>
<summary><b>🇬🇧 English Version (Click to expand)</b></summary>

# Pattern Recognition & Machine Learning: From Adversarial Examples to Generative Data Augmentation

## 1. Research Overview

Modern deep learning systems serve as critical infrastructure across computer vision, biometric security, medical imaging, and collaborative computing. However, deep learning models remain vulnerable to **adversarial attacks, privacy leakage, and data distribution shifts**.

Our research focuses on **Pattern Recognition and Machine Learning**, bridging **Adversarial Machine Learning (AML)** and **Generative Data Augmentation**. By understanding model vulnerabilities through perturbation design, we build secure, robust, privacy-preserving, and computationally efficient models.

## 2. Three Research Pillars

```
                   Research Scope
                        │
    ┌───────────────────┼───────────────────┐
    │                   │                   │
 1.Adversarial ML   2.Collaborative     3.Generative Models
    │              Training & Distill.    & Data Augment.
    │                   │                   │
 · Attack & Defense  · Federated Learning · Data Distillation
 · Detection &       · Knowledge          · PEFT & Synthesis
   Robustness          Distillation
```

---

### Pillar 1: Adversarial ML — Attack, Defense & Robustness

Investigating static and dynamic threats in open-world environments, balancing model utility and security.

| Direction | Key Achievements |
|:---|:---|
| **Query-Efficient Adversarial Attacks** | **DAIR**: a query-efficient decision-based black-box attack for CBIR systems, reducing query overhead by **87%** and bypassing Microsoft Bing (ACM SIGIR 2021) |
| **Model-Agnostic Adversarial Detection** | Detection via random perturbations on input space, leveraging output statistical change patterns to catch low-magnitude adversarial noise |
| **Ensemble & Feature Robustness** | **PDD** & **DEG**: multi-view base-network feature diversification to optimize ensemble robustness against gradient-based attacks (AAAI 2021) |

---

### Pillar 2: Collaborative Training, Federated Learning & Knowledge Distillation

Addressing non-IID (long-tailed) data, client heterogeneity, privacy leakage, and communication bottlenecks.

| Direction | Key Achievements |
|:---|:---|
| **Long-Tailed Federated Learning** | **FedHyb / FedDDL**: instance-based client sampling + class-balanced proxy distillation at server, resolving classifier bias under extreme non-IID (α=0.5, IF=100) (ECAI 2024) |
| **Adaptive Adversarial Distillation** | **AdaAD**: optimizes small-capacity student training via adversarial game framework with dynamic anchor-point search, boosting both accuracy and robustness (CVPR 2023) |
| **Privacy Inference & Leakage Auditing** | Demonstrated property inference, sample reconstruction, and membership inference in deep feature spaces during collaborative updates (IEEE ICME 2022) |
| **One-Shot Federated Learning** | **SEDAG**: single-round server aggregation via data-free multi-expert distillation, cutting communication costs and poisoning exposure |

---

### Pillar 3: Generative Models, Data Augmentation & Model Tuning

Leveraging GANs, Diffusion Models, and Auto-regressive Transformers to address data scarcity, domain shifts, and privacy constraints.

| Direction | Key Achievements |
|:---|:---|
| **Robustness Feature Adapter (RFA)** | Plug-and-play adapter generating dynamic adversarial perturbations. ViT adversarial training accelerated **>4×**, parameter overhead reduced to **<1/10**, robustness gains **>50%** (ECAI 2025) |
| **Influence-Guided Diffusion (IGD)** | Target-gradient guidance during reverse diffusion sampling for training-free, task-adaptive proxy dataset generation (ICLR 2025) |
| **Diffusion Reconstruction Likelihood** | DDPM partial-reconstruction deviations to estimate data likelihood for core-set selection, supporting incremental learning and edge deployment (AAAI 2026) |
| **Cross-Modal Medical Image Fusion** | **FedMCA**: cross-attention personalized multimodal FL for modality-heterogeneous MRI segmentation and classification (ICMSSP 2026) |
| **Metamaterial Inverse Design** | 3D Conditional Diffusion Models + topological derivative data augmentation for synthesizing metamaterial structures with specified elastic modulus and conductivity |

---

## 3. Core Philosophy: From Adversarial Examples to Generative Data Augmentation

```
  Adversarial                      Data
  Examples                    Augmentation
    │                              │
    ├── Learn effective perturbations in data space ───┤
    │                              │
    ├── Exploit "linear sensitivity" in high-dim space ─┤
    │                              │
    └── Enhance model robustness & generalization ──────┘
```

| Dimension | Adversarial Examples | Data Augmentation |
|:---|:---|:---|
| **Perturbation Goal** | Directed perturbation under constraints; goal is "to break model performance" | Natural perturbation under distribution constraints; goal is "to preserve semantics, add variation" |
| **Perturbation Method** | Directional accumulated perturbation causing misclassification | Micro-perturbations that don't alter semantics, only add diversity |
| **Core Value** | Exposes vulnerabilities via adversarial training; learns to counter security threats | Supplements training data to cover more scenarios; mitigates data scarcity and distribution shift |

> **Key Insight:** Model capability ceiling depends on data quality, structure, and organization.

---

## 4. Representative Publications

| Year | Title | Venue | Topic |
|:---|:---|:---|:---|
| 2026 | Diffusion Reconstruction-Based Data Likelihood Estimation for Core-Set Selection | **AAAI 2026** | Data Distillation / Diffusion |
| 2026 | FedMCA: Cross-Attention-Based Personalized Multimodal Federated Learning | **ICMSSP 2026** | Multimodal Medical FL |
| 2025 | Robustness Feature Adapter for Efficient Adversarial Training | **ECAI 2025** | Efficient Adv. Training / PEFT |
| 2025 | Influence-Guided Diffusion for Dataset Distillation | **ICLR 2025** | Generative Dataset Distillation |
| 2025 | StableGuard: Towards Unified Copyright Protection and Tamper Localisation | **NeurIPS 2025** | AI Safety & Watermarking |
| 2024 | Federated Learning with Hybrid Knowledge Distillations on Long-Tailed Data | **ECAI 2024** | Long-Tailed Federated Learning |
| 2023 | Boosting Accuracy and Robustness via Adaptive Adversarial Distillation | **CVPR 2023** | Adversarial Knowledge Distillation |
| 2022 | Individual Property Inference Over Collaborative Learning | **IEEE ICME 2022** | Privacy Leakage in FL |
| 2021 | DAIR: A Query-Efficient Decision-Based Attack On Image Retrieval | **ACM SIGIR 2021** | Black-Box CBIR Attack |
| 2021 | Adversarial Defence By Diversified Simultaneous Training Of Deep Ensembles | **AAAI 2021** | Deep Ensemble Robustness |

---

## 5. Grants & Intellectual Property

- **NSFC General Program:** Privacy and Security Issues in Biometric Recognition and Retrieval under Adversarial Environments (Grant No. 61876040, 650,000 RMB)
- **Guangdong Basic and Applied Basic Research Foundation:** Smart Processing of Vital Sign Signals at the Edge (Co-PI with Sun Yat-sen University)
- **Patents:** Multiple US and Chinese National Invention Patents on adversarial detection, secure hashing retrieval, and privacy-preserving federated training

---

## 6. Contact

- **Affiliation:** School of Computer Science and Technology, Dongguan University of Technology (Songshan Lake Campus)
- **Email:** wangyi@dgut.edu.cn

</details>

---

> **使用说明：** 点击上方 `<details>` 折叠区域标题即可展开对应语言版本。在支持 HTML 渲染的 Markdown 阅读器（如 GitHub、VS Code 预览、Typora）中效果最佳。
>
> **Usage:** Click the `<details>` section headers above to expand the language version you need. Works best in Markdown renderers with HTML support (GitHub, VS Code preview, Typora, etc.).
