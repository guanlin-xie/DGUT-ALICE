---
widget: blank
headless: true

# ... Put Your Section Options Here (title etc.) ...
title: Research
subtitle:
weight: 10  # section position on page
design:
  # Choose how many columns the section has. Valid values: 1 or 2.
  columns: '1'
---
<style>
  .wrap{max-width:920px;margin:0 auto;padding:0 6px 40px;font-size:16.5px;line-height:1.85;color:#2b2b2b;}
  .wrap.lang-zh .en{display:none !important;}
  .wrap.lang-en .zh{display:none !important;}
  .hero{position:relative;padding:34px 0 26px;border-bottom:1px solid #e5e5e5;text-align:center;}
  .kicker{font-size:13px;letter-spacing:.18em;text-transform:uppercase;color:#8a8a8a;margin-bottom:14px;}
  .title{font-size:30px;line-height:1.4;font-weight:700;margin:0 0 14px;color:#1a1a1a;}
  .meta{font-size:14.5px;color:#6d6d6d;margin-top:4px;}
  .toggle{position:fixed;top:86px;right:22px;z-index:999;padding:6px 14px;font-size:13px;letter-spacing:.06em;color:#fff;background:#2f5d8a;border:1px solid #2f5d8a;border-radius:999px;cursor:pointer;box-shadow:0 2px 8px rgba(0,0,0,.16);}
  .toggle:hover{background:#24486b;}
  .lead{margin:26px 0 6px;color:#3a3a3a;}
  .toc{margin:18px 0 6px;padding:16px 20px;background:#f7f8fa;border-left:3px solid #2f5d8a;border-radius:2px;}
  .toc-title{font-size:13px;letter-spacing:.14em;color:#8a8a8a;text-transform:uppercase;margin-bottom:8px;}
  .toc ol{margin:0;padding-left:20px;}
  .toc li{margin:3px 0;}
  .toc a{color:#2f5d8a;text-decoration:none;}
  .toc a:hover{text-decoration:underline;}
  .sec{margin:52px 0 0;scroll-margin-top:96px;}
  .sec-head{display:flex;align-items:baseline;gap:14px;border-bottom:2px solid #1a1a1a;padding-bottom:10px;margin-bottom:8px;}
  .sec-no{font-size:13px;letter-spacing:.16em;color:#2f5d8a;font-weight:700;white-space:nowrap;}
  .sec-head h2{font-size:24px;margin:0;font-weight:700;color:#1a1a1a;line-height:1.35;}
  .chips{margin:12px 0 4px;}
  .chip{display:inline-block;margin:4px 8px 4px 0;padding:3px 11px;font-size:12.5px;color:#444;background:#eef2f6;border:1px solid #dde4ec;border-radius:999px;}
  .sub{margin:34px 0 0;}
  .sub h3{font-size:18.5px;font-weight:700;color:#1a1a1a;margin:0 0 8px;padding-left:12px;border-left:4px solid #2f5d8a;line-height:1.5;}
  .sub p{margin:8px 0;}
  .sub ul{margin:8px 0 8px;padding-left:22px;}
  .sub li{margin:4px 0;}
  .pub{margin-top:10px;padding:9px 14px;font-size:13px;color:#5c6672;background:#fafafa;border-left:2px solid #c9d2dc;line-height:1.7;}
.fig{margin:22px 0 4px;text-align:center;}
.fig img{display:block;margin:0 auto;height:auto;max-width:100%;border:1px solid #ececec;background:#fff;}
.fig.narrow img{max-width:62%;}
.fig.mid img{max-width:80%;}
.fig.wide img{max-width:100%;}
.cap{margin-top:8px;font-size:13px;color:#6d6d6d;line-height:1.65;text-align:center;}
  .cards{display:grid;grid-template-columns:repeat(2,1fr);gap:14px;margin:18px 0 6px;}
  .card{padding:16px 18px;border:1px solid #e3e7ec;border-radius:4px;background:#fcfcfd;}
  .card h4{margin:0 0 6px;font-size:16px;color:#1a1a1a;}
  .card p{margin:0;font-size:13.5px;color:#606a75;line-height:1.7;}
  .card a{color:#2f5d8a;text-decoration:none;font-weight:600;}
  table.table{width:100%;border-collapse:collapse;margin:18px 0 8px;font-size:14.5px;}
  table.table th,table.table td{border:1px solid #e3e7ec;padding:10px 12px;vertical-align:top;text-align:left;}
  table.table th{background:#f3f5f8;font-weight:700;color:#1a1a1a;}
  table.table td:first-child{width:17%;background:#fafbfc;font-weight:600;color:#333;}
  .note{margin:22px 0 0;padding:16px 20px;background:#f7f8fa;border-radius:3px;border-left:3px solid #2f5d8a;font-size:15.5px;color:#2b2b2b;}
  .quote{margin:26px 0 0;text-align:center;font-size:17px;font-weight:600;color:#1a1a1a;letter-spacing:.02em;}
  .contact{margin-top:44px;padding-top:20px;border-top:1px solid #e5e5e5;text-align:center;color:#6d6d6d;font-size:14.5px;}
  .contact a{color:#2f5d8a;text-decoration:none;}
  @media (max-width:720px){
    .wrap{font-size:15.5px;}
    .title{font-size:23px;}
    .cards{grid-template-columns:1fr;}
    .toggle{top:auto;bottom:18px;right:18px;}
    .fig.narrow img,.fig.mid img{max-width:100%;}
  }
</style>
<div class="wrap lang-zh" id="r2">
<div class="hero">
<button id="toggle" class="toggle" type="button" data-lang="zh">EN</button>
</div>
<p class="lead zh">研究以模式识别与机器学习为主线，二十余年的积累串成一条从数据到模型的完整链条：从多元数据分析与可视化起步，进入对抗样本的生成与防御、协同训练与知识蒸馏，最终走向生成模型与数据增强。对抗样本揭示模型的脆弱之处，生成式数据增强则把这种敏感性转化为可用的多样性——两者指向同一个目标：以更优质的数据与更稳健的学习过程，提升模型的鲁棒性与泛化能力。</p>
<p class="lead en">Research centres on pattern recognition and machine learning, where two decades of work form a single chain from data to model: multivariate data analysis and visualization first, then the generation and defense of adversarial examples, then collaborative training and knowledge distillation, and finally generative models and data augmentation. Adversarial examples expose where a model is fragile; generative data augmentation turns that same sensitivity into usable diversity — both serving one goal: better data and more robust learning, for models that are accurate, resilient and generalizable.</p>
<div class="toc">
<div class="toc-title"><span class="zh">目录 / Contents</span><span class="en">Contents</span></div>
<ol>
<li><a href="#overview"><span class="zh">研究领域总览</span><span class="en">Research Overview</span></a></li>
<li><a href="#adversarial-examples"><span class="zh">Ⅰ 对抗样本的生成与防御</span><span class="en">Ⅰ Generating and Defending Adversarial Examples</span></a></li>
<li><a href="#collaborative-distillation"><span class="zh">Ⅱ 协同训练与知识蒸馏</span><span class="en">Ⅱ Collaborative Training and Knowledge Distillation</span></a></li>
<li><a href="#generative-augmentation"><span class="zh">Ⅲ 生成模型与数据增强</span><span class="en">Ⅲ Generative Models and Data Augmentation</span></a></li>
<li><a href="#summary"><span class="zh">总结：从对抗样本到生成式数据增强</span><span class="en">Summary: From Adversarial Examples to Generative Data Augmentation</span></a></li>
</ol>
</div>
<br>

<!-- overview -->
<div class="sec" id="overview">
<div class="sec-head"><span class="sec-no"></span><h2><span class="zh">研究领域总览</span><span class="en">Research Overview</span></h2></div>
<p class="zh">研究领域为模式识别与机器学习，形成四个相互支撑的板块，时间跨度自 2005 年延续至今：</p>
<p class="en">Research centres on pattern recognition and machine learning, organized into four mutually supporting blocks that span from 2005 to the present:</p>
<div class="cards">
<div class="card"><h4><span class="zh">多元数据分析与可视化</span><span class="en">Multivariate Data Analysis &amp; Visualization</span></h4><p><span class="zh">指纹方向场建模；去噪、重建与检索；基于 GLM 与多种重采样方法的高维离散数据统计分析工具包 mvabund，被收录进 CRAN 国际档案大全。</span><span class="en">Fingerprint orientation-field modelling; denoising, reconstruction and retrieval; the mvabund toolbox for high-dimensional discrete data built on GLM and multiple resampling methods, archived in CRAN.</span></p></div>
<div class="card"><h4><span class="zh"><a href="#adversarial-examples">对抗样本的生成与防御</a></span><span class="en"><a href="#adversarial-examples">Generating and Defending Adversarial Examples</a></span></h4><p><span class="zh">对抗机器学习（AML）、对抗训练、对抗检索；生物特征隐私保护；查询安全高效的 CBIR 图像检索系统。</span><span class="en">Adversarial machine learning (AML), adversarial training and adversarial retrieval; biometric privacy protection; query-secure and query-efficient CBIR systems.</span></p></div>
<div class="card"><h4><span class="zh"><a href="#collaborative-distillation">协同训练与知识蒸馏</a></span><span class="en"><a href="#collaborative-distillation">Collaborative Training &amp; Knowledge Distillation</a></span></h4><p><span class="zh">联邦学习、模型蒸馏、数据集蒸馏；师生模型与对抗蒸馏。</span><span class="en">Federated learning, model distillation and dataset distillation; teacher–student models and adversarial distillation.</span></p></div>
<div class="card"><h4><span class="zh"><a href="#generative-augmentation">生成模型与数据增强</a></span><span class="en"><a href="#generative-augmentation">Generative Models &amp; Data Augmentation</a></span></h4><p><span class="zh">数据增强、参数高效微调（PEFT）；GAN、自回归 Transformer 与扩散模型驱动的数据生成。</span><span class="en">Data augmentation and parameter-efficient fine-tuning (PEFT); data generation driven by GANs, autoregressive Transformers and diffusion models.</span></p></div>
</div>
</div>
<br>


<!-- adversarial-examples -->
<div class="sec" id="adversarial-examples">
<div class="sec-head"><span class="sec-no"></span><h2><span class="zh">Ⅰ · 对抗样本的生成与防御</span><span class="en">Ⅰ · Generating and Defending Adversarial Examples</span></h2></div>
<div class="chips"><span class="chip zh">对抗机器学习</span><span class="chip en">Adversarial ML</span><span class="chip zh">对抗训练</span><span class="chip en">Adversarial training</span><span class="chip zh">对抗检索</span><span class="chip en">Adversarial retrieval</span></div>

<div class="sub">
<h3><span class="zh">对抗机器学习</span><span class="en">Adversarial Machine Learning</span></h3>
<p class="zh">传统机器学习建立在“静态环境”的平稳性假设之上；真实开放环境打破这一假设，攻击者可通过数据投毒、白盒攻击、黑盒攻击与绕过检测等手段破坏模型。</p>
<p class="en">Classical machine learning rests on a stationarity assumption about a static environment. Real open-world deployment breaks that assumption: attackers can poison data, mount white-box or black-box attacks, or bypass detection.</p>
<ul class="zh">
<li><strong>平稳性假设</strong>：训练/测试数据独立同分布，统计特性不随时间改变。</li>
<li><strong>该假设支撑</strong>：模型有效性、预测可靠性、统计检验性。</li>
<li><strong>开放环境</strong>：对抗样本的生成与防御成为模型落地的必要环节。</li>
</ul>
<ul class="en">
<li><strong>Stationarity assumption</strong>: training and test data are i.i.d., and statistical properties do not drift over time.</li>
<li><strong>What it underpins</strong>: model validity, prediction reliability and statistical testability.</li>
<li><strong>Open environment</strong>: generating and defending adversarial examples becomes indispensable for deployment.</li>
</ul>
<div class="fig mid">
<img src="fig01.png" alt="Figure 1 Stationarity: model reliability and statistical testability hold only when training and test data share one distribution">
<div class="cap"><span class="zh">图1 平稳性假设：训练数据与测试数据同分布，是模型可靠性与统计检验性成立的前提。</span><span class="en">Figure 1 Stationarity: model reliability and statistical testability hold only when training and test data share one distribution.</span></div>
</div>
</div>
<br>


<div class="sub">
<h3><span class="zh">基于内容查询的图像检索攻击</span><span class="en">Attacking Content-Based Image Retrieval</span></h3>
<p class="zh">针对 CBIR 系统提出一种自适应的决策型黑盒算法，大幅减少 87% 的系统查询次数，并在微软必应 Bing 等商业检索引擎上展示了攻击有效性：原始图像的检索结果（如 wardrobe）被对抗样本整体改写为 tapestry、painting、tiles 等无关结果。</p>
<p class="en">For CBIR systems we propose an adaptive decision-based black-box algorithm that cuts system queries by 87%, and demonstrate its effectiveness on commercial engines such as Microsoft Bing: the original retrieval results (e.g. wardrobe) are rewritten by an adversarial sample into unrelated results such as tapestry, painting and tiles.</p>
<ul class="zh">
<li>查询高效：决策型黑盒设定下大幅压缩查询预算。</li>
<li>真实可用：在商业视觉检索（Bing 相似图片）上验证。</li>
<li>面向检索：攻击目标是 top-K 检索结果，而非单一分类标签。</li>
</ul>
<ul class="en">
<li>Query-efficient: sharply reducing the query budget under a decision-based black-box setting.</li>
<li>Practically valid: verified on a commercial visual search engine (Bing Similar Images).</li>
<li>Retrieval-oriented: the target is the top-K retrieved set, not a single class label.</li>
</ul>
<div class="fig mid">
<img src="fig02.png" alt="Figure 2 The black-box attack validated on Microsoft Bing visual search, a commercial CBIR system">
<div class="cap"><span class="zh">图2 在微软必应视觉检索（商业 CBIR 系统）上验证黑盒攻击的有效性。</span><span class="en">Figure 2 The black-box attack validated on Microsoft Bing visual search, a commercial CBIR system.</span></div>
</div>
<div class="pub">M. Chen, J. Lu, Y. Wang, J. Qin and W. Wang. “DAIR: A Query-Efficient Decision-Based Attack On Image Retrieval Systems”, <em>ACM SIGIR’21</em> [C], 2021, Virtual Event, 1064–1073.</div>
</div>
<br>


<div class="sub">
<h3><span class="zh">联邦学习中的数据重构与隐私泄露</span><span class="en">Data Reconstruction and Privacy Leakage in Federated Learning</span></h3>
<p class="zh">根据客户端上传到服务器的信息，对其本地数据集实施隐私保护攻击，包括样本重构、参数泄漏、成员推断与属性推断等。</p>
<p class="en">From the information clients upload to the server, we mount privacy attacks on their local datasets — sample reconstruction, parameter leakage, membership inference and property inference.</p>
<ul class="zh">
<li>揭示了协同学习中“共享参数”并不等于“共享安全”。</li>
<li>在深度特征空间对客户端本地数据集进行属性推断。</li>
<li>给出客户端样本重构的准确率比较，量化泄露风险。</li>
</ul>
<ul class="en">
<li>Shows that sharing parameters in collaborative learning is not the same as sharing safety.</li>
<li>Performs property inference on a client’s local dataset in deep feature space.</li>
<li>Reports client-side sample reconstruction accuracy to quantify the leakage risk.</li>
</ul>
<div class="fig wide">
<img src="fig03.png" alt="Figure 3 Privacy leakage in federated learning: uploaded model information enables property inference and sample reconstruction">
<div class="cap"><span class="zh">图3 联邦学习中的隐私泄露路径：客户端上传的模型信息被用于属性推断与样本重构。</span><span class="en">Figure 3 Privacy leakage in federated learning: uploaded model information enables property inference and sample reconstruction.</span></div>
</div>
<div class="pub">H. Yang, Y. Wang and B. Li. “Individual Property Inference Over Collaborative Learning In Deep Feature Space”, <em>IEEE ICME’22</em> [C], 2022, Taipei, Taiwan, 1–6.</div>
</div>
<br>


<div class="sub">
<h3><span class="zh">集成深度模型的对抗稳健性</span><span class="en">Adversarial Robustness of Deep Ensembles</span></h3>
<p class="zh">基模型高层特征的多样化表示可以显著提升集成深度学习模型的对抗稳健性，据此提出优先多样化 Dropout（PDD）与分散式集成梯度（DEG）。</p>
<p class="en">Diversified high-level feature representations across base networks markedly improve the adversarial robustness of deep ensembles — realized as Priority Diversified Dropout (PDD) and Dispersed Ensemble Gradients (DEG).</p>
<ul class="zh">
<li>以 Grad-CAM 可视化对比基线、ADP 与 PDD 下各基网络对最后一层 FC 的关注区域。</li>
<li>CIFAR-100 上 2000 张测试图像的平均判别分数箱线图：分数越高，基网络间 FC 特征差异越大（K = 3）。</li>
</ul>
<ul class="en">
<li>Grad-CAM comparison of the last fully-connected layer for each base network under baseline, ADP and PDD.</li>
<li>Box-plots of the average discrimination score over 2000 CIFAR-100 test images — a higher value means larger FC-feature divergence among base networks (K = 3).</li>
</ul>
<div class="fig mid">
<img src="fig04.png" alt="Figure 4 Grad-CAM of the last FC layer in each base network: (a) baseline, (b) ADP, (c) PDD (ours)">
<div class="cap"><span class="zh">图4 集成模型中各基网络最后一层 FC 的 Grad-CAM 对比：(a) 基线、(b) ADP、(c) PDD（本文方法）。</span><span class="en">Figure 4 Grad-CAM of the last FC layer in each base network: (a) baseline, (b) ADP, (c) PDD (ours).</span></div>
</div>
<div class="pub">B. Huang, Z. Ke, Y. Wang, W. Wang, L. Shen and F. Liu. “Adversarial Defence By Diversified Simultaneous Training Of Deep Ensembles”, <em>AAAI’21</em> [C], 2021, Virtual Event, 35(9), 7823–7831.</div>
</div>
</div>
<br>


<!-- collaborative-distillation -->
<div class="sec" id="collaborative-distillation">
<div class="sec-head"><span class="sec-no"</span><h2><span class="zh">Ⅱ · 协同训练与知识蒸馏</span><span class="en">Ⅱ · Collaborative Training and Knowledge Distillation</span></h2></div>
<div class="chips"><span class="chip zh">联邦学习</span><span class="chip en">Federated learning</span><span class="chip zh">师生模型</span><span class="chip en">Teacher–student models</span><span class="chip zh">模型蒸馏</span><span class="chip en">Model distillation</span><span class="chip zh">对抗蒸馏</span><span class="chip en">Adversarial distillation</span></div>
<p class="zh">该方向关注的核心矛盾是：多客户端长尾数据导致协作偏差并影响收敛。研究围绕隐私—效用与通信效率、模型鲁棒性与泛化能力、多模态表征对齐与多路编码器融合、多场景应用下的模型泛化与自适应能力展开。</p>
<p class="en">The central tension: long-tailed data across many clients induces collaboration bias and hurts convergence. Research addresses privacy–utility and communication efficiency, model robustness and generalization, multimodal representation alignment and multi-encoder fusion, and cross-scenario generalization and adaptivity.</p>


<div class="sub">
<h3><span class="zh">联邦蒸馏解决长尾数据分布导致的协作偏差</span><span class="en">Federated Distillation against Long-Tailed Collaboration Bias</span></h3>
<p class="zh">多客户端数据呈现长尾分布（Non-IID），带来安全隐私保护、客户端过拟合、收敛慢且不稳定、策略异质性四类挑战；以“联邦蒸馏 + 数据增强”应对：基于实例的自然采样与基于类别的均衡采样协同，在服务器端优化聚合与平滑统计，并对分类器偏差进行校准。</p>
<p class="en">Client data are long-tailed (Non-IID), raising four challenges — privacy protection, client over-fitting, slow and unstable convergence, and strategy heterogeneity. The answer is federated distillation plus data augmentation: instance-based natural sampling combined with class-based balanced sampling, server-side optimization of aggregation and smoothed statistics, and calibration of classifier bias.</p>
<ul class="zh">
<li>更适合表示学习的采样与更适合分类器学习的采样互补。</li>
<li>针对分类器偏差与泛化能力不足进行显式校准。</li>
</ul>
<ul class="en">
<li>Samples better suited to representation learning complement those better suited to classifier learning.</li>
<li>Explicit calibration against classifier bias and limited generalization.</li>
</ul>
<div class="fig narrow">
<img src="fig05.png" alt="Figure 5 Class distribution of client data: the long tail induces collaboration bias and classifier bias">
<div class="cap"><span class="zh">图5 客户端本地数据的类别分布示意：长尾导致协作偏差与分类器偏置。</span><span class="en">Figure 5 Class distribution of client data: the long tail induces collaboration bias and classifier bias.</span></div>
</div>
</div>
<br>


<div class="sub">
<h3><span class="zh">客户端自蒸馏</span><span class="en">Client Self-Distillation</span></h3>
<p class="zh">通过引入随机变换生成的蒸馏数据，并结合多个子网络的软标签对齐（Logits Transfer），增强模型内部知识多样性，抑制本地过拟合。</p>
<p class="en">Randomly transformed distillation data, combined with soft-label alignment (logits transfer) across multiple sub-networks, strengthens intra-model knowledge diversity and suppresses local over-fitting.</p>
<div class="fig wide">
<img src="fig06.png" alt="Figure 6 Client self-distillation: distillation data from random transforms, with logits transfer across sub-networks to curb local over-fitting">
<div class="cap"><span class="zh">图6 客户端自蒸馏：随机变换生成蒸馏数据，并通过多个子网络的软标签对齐抑制本地过拟合。</span><span class="en">Figure 6 Client self-distillation: distillation data from random transforms, with logits transfer across sub-networks to curb local over-fitting.</span></div>
</div>
</div>
<br>


<div class="sub">
<h3><span class="zh">服务器集成蒸馏</span><span class="en">Server Ensemble Distillation</span></h3>
<p class="zh">通过类别均衡的第三方无标签代理数据集引导多方位知识迁移，对齐师生模型在其上的特征表示与软标签；三重对齐模型权重、特征表示与软标签输出，学习更紧凑的特征并优化损失空间结构，提升全局模型的鲁棒性和泛化能力。</p>
<p class="en">A class-balanced, third-party unlabeled proxy dataset steers multi-faceted knowledge transfer, aligning teacher and student representations and soft labels on it. Triple alignment — model weights, feature representations and soft-label outputs — yields more compact features and a better-structured loss space, improving global robustness and generalization.</p>
<div class="fig wide">
<img src="fig07.png" alt="Figure 7 Server ensemble distillation (FedHyb): weight, feature and logits aggregation on a class-balanced unlabeled proxy dataset">
<div class="cap"><span class="zh">图7 服务器集成蒸馏（FedHyb）：在类别均衡的无标签代理数据集上做权重、特征与软标签三重聚合。</span><span class="en">Figure 7 Server ensemble distillation (FedHyb): weight, feature and logits aggregation on a class-balanced unlabeled proxy dataset.</span></div>
</div>
<div class="pub">S. Liu, Y. Zhang, K. Zhang and Y. Wang. “Federated Learning with Hybrid Knowledge Distillations on Long-Tailed Heterogeneous Client Data”, <em>ECAI’24</em> [C], 2024, Santiago de Compostela, Spain, vol. 392, 2878–2885.</div>
</div>
<br>


<div class="sub">
<h3><span class="zh">突破联邦学习在长尾异构下的性能瓶颈</span><span class="en">Breaking the Long-Tailed Heterogeneity Bottleneck</span></h3>
<p class="zh">在不同数据异质性指标 α 与长尾分布指标 IF 下，所提方法在 SVHN、CIFAR-10 以及医学影像基准数据集 CheXpert 上均取得更高的全局测试准确率。</p>
<p class="en">Across data-heterogeneity level α and long-tail indicator IF, the method achieves higher global test accuracy on SVHN, CIFAR-10 and the medical imaging benchmark CheXpert.</p>
<ul class="zh">
<li>达到目标精度所需的通信轮次显著减少。</li>
<li>对恶意客户端下的毒攻击更鲁棒（随机噪声攻击、拜占庭攻击）。</li>
</ul>
<ul class="en">
<li>Markedly fewer communication rounds to reach a target accuracy.</li>
<li>More robust to poisoning by malicious clients (random-noise and Byzantine attacks).</li>
</ul>
<div class="fig narrow">
<img src="fig08.png" alt="Figure 8 Global accuracy under random-noise attackers: the proposed method is best at every attack strength">
<div class="cap"><span class="zh">图8 随机噪声攻击下的全局准确率：所提方法在各攻击强度下均最优。</span><span class="en">Figure 8 Global accuracy under random-noise attackers: the proposed method is best at every attack strength.</span></div>
</div>
</div>
<br>


<div class="sub">
<h3><span class="zh">自适应的对抗蒸馏法（AdaAD）</span><span class="en">Adaptive Adversarial Distillation (AdaAD)</span></h3>
<p class="zh">传统对抗训练在小容量学生模型上提升鲁棒性并不理想，常出现精度与鲁棒性失衡。AdaAD 在对抗博弈框架下优化大小模型之间的蒸馏过程：模拟近似推导二者的最大点对点对齐关系，在内部优化中自适应搜索最优匹配点（锚点），通过小模型生成对抗训练数据以增加大小模型间互动，并设计新的对抗蒸馏目标。</p>
<p class="en">Conventional adversarial training struggles on small-capacity students, often trading accuracy for robustness. AdaAD optimizes teacher–student distillation inside an adversarial-game framework: it derives the maximal point-to-point alignment between the two models, adaptively searches for the best anchor during inner optimization, generates adversarial training data through the student to increase interaction, and designs a new adversarial distillation objective.</p>
<div class="fig mid">
<img src="fig09.png" alt="Figure 9 The AdaAD teacher–student distillation framework with adaptive anchor search">
<div class="cap"><span class="zh">图9 AdaAD 的师生蒸馏框架与自适应锚点搜索过程。</span><span class="en">Figure 9 The AdaAD teacher–student distillation framework with adaptive anchor search.</span></div>
</div>
<div class="pub">B. Huang, M. Chen, Y. Wang, J. Lu, M. Cheng and W. Wang. “Boosting Accuracy and Robustness Of Student Models Via Adaptive Adversarial Distillation”, <em>IEEE/CVF CVPR’23</em> [C], 2023, Vancouver, Canada, 24668–24677.</div>
</div>
</div>
<br>


<!-- generative-augmentation -->
<div class="sec" id="generative-augmentation">
<div class="sec-head"><span class="sec-no"></span><h2><span class="zh">Ⅲ · 生成模型与数据增强</span><span class="en">Ⅲ · Generative Models and Data Augmentation</span></h2></div>
<div class="chips"><span class="chip zh">数据增强</span><span class="chip en">Data augmentation</span><span class="chip zh">数据集蒸馏</span><span class="chip en">Dataset distillation</span><span class="chip zh">参数高效微调（PEFT）</span><span class="chip en">Parameter-efficient fine-tuning</span></div>


<div class="sub">
<h3><span class="zh">图像生成模型</span><span class="en">Image Generation Models</span></h3>
<p class="zh">涵盖生成式对抗网络 GAN、自回归 Transformer 与 Diffusion 扩散模型三条技术路线，面向四类需求：满足小样本学习、符合常理和常识、减少算力和内存、具备局部编辑可控性——即可靠、鲁棒、高效。</p>
<p class="en">Three technical routes — GANs, autoregressive Transformers and diffusion models — serve four requirements: few-shot capability, commonsense plausibility, reduced compute and memory, and controllable local editing, i.e. reliable, robust and efficient generation.</p>
<div class="fig mid">
<img src="fig10.png" alt="Figure 10 Controllable editing with image generation models: new styles, new shape, new texture">
<div class="cap"><span class="zh">图10 图像生成模型的可控编辑：新风格、形状与新纹理。</span><span class="en">Figure 10 Controllable editing with image generation models: new styles, new shape, new texture.</span></div>
</div>
</div>
<br>


<div class="sub">
<h3><span class="zh">生成式数据增强：对抗数据增强</span><span class="en">Generative Augmentation: Adversarial Data Augmentation</span></h3>
<p class="zh">在主网络中插入鲁棒特征适配器（RFA），通过在特征空间动态自适应生成对抗扰动，有效解决传统对抗训练计算开销大和鲁棒过拟合的问题；推理阶段插拔 RFA 适配器还可用于对抗检测。</p>
<p class="en">A Robustness Feature Adapter (RFA) inserted into the main network dynamically generates adversarial perturbations in feature space, solving the high computational cost and robust over-fitting of conventional adversarial training; the adapter can be plugged in or out at inference for adversarial detection.</p>
<ul class="zh">
<li>ViT 对抗训练效率提升 4 倍以上。</li>
<li>模型复杂度增加不足 1/10，鲁棒性增益可超过 50%。</li>
</ul>
<ul class="en">
<li>Over 4× faster adversarial training for ViT.</li>
<li>Less than 1/10 added model complexity, with robustness gains above 50%.</li>
</ul>
<div class="fig mid">
<img src="fig11.png" alt="Figure 11 Where RFA is inserted, and its training/inference flow: only adapter parameters are updated to generate perturbations">
<div class="cap"><span class="zh">图11 RFA 的插入位置与训练/推理流程：仅更新适配器参数即可生成对抗扰动。</span><span class="en">Figure 11 Where RFA is inserted, and its training/inference flow: only adapter parameters are updated to generate perturbations.</span></div>
</div>
<div class="pub">Q. Wu, J. Guo, W. Wang and Y. Wang. “Robustness Feature Adapter for Efficient Adversarial Training”, <em>ECAI’25</em> [C], 2025, Bologna, Italy, vol. 413, 3451–3459.</div>
</div>
<br>


<div class="sub">
<h3><span class="zh">“插件式”RFA 对抗训练的收敛质量与效率</span><span class="en">Convergence Quality and Efficiency of Plug-in RFA</span></h3>
<p class="zh">从效率与收敛质量两方面评估 RFA：仅更新适配器参数即可显著降低计算开销，尤其适用于大规模预训练模型（如 ViT）的对抗训练；尽管训练速度快，仍能保持较低的 FOSC 值，说明生成的对抗样本质量高，有助于提升鲁棒性泛化能力。该结构亦可迁移至个性化联邦学习，同时增强客户端对抗鲁棒性。</p>
<p class="en">RFA is evaluated on both efficiency and convergence quality: updating only adapter parameters sharply cuts computation, especially for large pre-trained models such as ViT; despite fast training it maintains a low FOSC value, indicating high-quality adversarial examples that improve robustness generalization. The same design transfers to personalized federated learning while strengthening client-side adversarial robustness.</p>
<div class="fig mid">
<img src="fig12.png" alt="Figure 12 Training time per batch vs FOSC: efficiency together with adversarial-sample quality">
<div class="cap"><span class="zh">图12 每批次训练时间与 FOSC 的关系：兼顾训练效率与对抗样本质量。</span><span class="en">Figure 12 Training time per batch vs FOSC: efficiency together with adversarial-sample quality.</span></div>
</div>
</div>
<br>


<div class="sub">
<h3><span class="zh">生成式数据增强：自适应下游多任务模型</span><span class="en">Generative Augmentation: Adapting to Downstream Multi-Task Models</span></h3>
<p class="zh">情景自适应的数据增强（IGD）在推理阶段利用外部约束（目标梯度），引导反向扩散过程动态自适应地生成能够等效训练下游任务模型的代理数据集，实现生成模型免微调、高效率地控制反向去噪过程。</p>
<p class="en">Scene-adaptive data augmentation (IGD) uses external constraints — target gradients — at inference time to steer the reverse diffusion process, dynamically generating a proxy dataset that can equivalently train downstream models. The generative model needs no fine-tuning, and the reverse denoising process is controlled efficiently.</p>
<ul class="zh">
<li>设计自定义的外部属性梯度作为引导函数。</li>
<li>在反向去噪的推断采样阶段施加定向吸引力或排斥力。</li>
<li>引导生成过程自适应下游任务目标，避免昂贵的生成模型重训练。</li>
</ul>
<ul class="en">
<li>A custom external attribute gradient serves as the guidance function.</li>
<li>Directed attraction or repulsion is applied during inference-time reverse denoising.</li>
<li>Generation adapts to the downstream objective, avoiding costly retraining of the generator.</li>
</ul>
<div class="fig wide">
<img src="fig13.png" alt="Figure 13 Real samples (left of the dashed line) vs generated proxy samples (right)">
<div class="cap"><span class="zh">图13 真实样本（虚线左）与生成的代理样本（虚线右）对比。</span><span class="en">Figure 13 Real samples (left of the dashed line) vs generated proxy samples (right).</span></div>
</div>
<div class="pub">M. Chen, J. Du, B. Huang, Y. Wang, X. Zhang and W. Wang. “Influence-Guided Diffusion for Dataset Distillation”, <em>ICLR’25</em> [C], 2025, Singapore, 1287–1308.</div>
</div>
<br>


<div class="sub">
<h3><span class="zh">生成式数据增强：数据蒸馏代表性样本</span><span class="en">Generative Augmentation: Representative Samples via Data Distillation</span></h3>
<p class="zh">核心数据集蒸馏法（Core-Set Selection）将大型真实数据集的核心知识提炼到小规模合成或筛选数据集，可用于持续/增量学习与边缘设备部署；通过 DDPM 部分逆去噪过程中引发的重建偏差，反映并量化潜在的数据似然度。</p>
<p class="en">Core-set selection distils the core knowledge of a large real dataset into a small synthesized or selected set, serving continual/incremental learning and edge deployment. Reconstruction bias induced by partial reverse denoising in DDPM reflects and quantifies the underlying data likelihood.</p>
<ul class="zh">
<li>高似然样本：重构偏差小。</li>
<li>低似然样本：语义变化、视觉显著性下降。</li>
<li>选择最优重建时刻 t，使目标落在给定区间内。</li>
</ul>
<ul class="en">
<li>High-likelihood samples: small reconstruction bias.</li>
<li>Low-likelihood samples: semantic drift and declining visual saliency.</li>
<li>Select the optimal reconstruction step t so that the target falls within the required interval.</li>
</ul>
<div class="fig wide">
<img src="fig14.png" alt="Figure 14 Data likelihood estimated from the reconstruction deviation of partial reverse denoising, yielding the optimal reconstruction timestep t">
<div class="cap"><span class="zh">图14 以部分逆去噪的重建偏差估计数据似然度，并据此确定最优重建时刻 t。</span><span class="en">Figure 14 Data likelihood estimated from the reconstruction deviation of partial reverse denoising, yielding the optimal reconstruction timestep t.</span></div>
</div>
<div class="pub">M. Chen, J. Du, B. Huang, Y. Wang, X. Zhang and W. Wang. “Diffusion Reconstruction-based Data Likelihood Estimation for Core-Set Selection”, <em>AAAI’26</em> [C], 2026, Singapore.</div>
</div>
<br>


<div class="sub">
<h3><span class="zh">生成式数据增强：多模态医学图像融合</span><span class="en">Generative Augmentation: Multimodal Medical Image Fusion</span></h3>
<p class="zh">通过多模态特征融合与分布对齐的协同优化，提高模型对复杂异构数据的表征能力，从而提升整体预测精度。</p>
<p class="en">Coordinated multimodal feature fusion and distribution alignment strengthen the model’s representation of complex heterogeneous data, raising overall predictive accuracy.</p>
<div class="fig mid">
<img src="fig15.png" alt="Figure 15 Multimodal federated methods on CheXpert (FedMCA is ours)">
<div class="cap"><span class="zh">图15 CheXpert 上的多模态联邦方法对比（FedMCA 为本团队方法）。</span><span class="en">Figure 15 Multimodal federated methods on CheXpert (FedMCA is ours).</span></div>
</div>
<div class="pub">Y. Zhang, S. Liu, B. Fang and Y. Wang. “FedMCA: Cross-Attention-Based Personalized Multimodal Federated Learning Under Modality Heterogeneity”, <em>ICMSSP’26</em> [C], 2026, Hiroshima, Japan.</div>
</div>
<br>


<div class="sub">
<h3><span class="zh">生成式数据增强：单轮通信的联邦学习</span><span class="en">Generative Augmentation: One-Shot Communication Federated Learning</span></h3>
<p class="zh">数据生成阶段基于对抗博弈的多专家蒸馏融合客户端编码器；模型蒸馏阶段将融合后的集成编码器知识蒸馏到全局模型。由此服务器可通过单轮通信学习全局模型，有效降低客户端的通信成本与安全风险。</p>
<p class="en">In the data-generation stage, multi-expert distillation under an adversarial game fuses client encoders; in the model-distillation stage, the fused ensemble-encoder knowledge is distilled into the global model. The server can therefore learn a global model in a single communication round, cutting client communication cost and security risk.</p>
<ul class="zh">
<li>无需额外信息交换：只需在客户端与服务器之间传输模型参数。</li>
<li>无需辅助数据集（data-free）：服务器不需要额外的训练数据。</li>
<li>考虑模型异质性：适应不同客户端拥有不同的模型架构。</li>
</ul>
<ul class="en">
<li>No extra information exchange: only model parameters travel between clients and server.</li>
<li>No auxiliary dataset (data-free): the server needs no additional training data.</li>
<li>Model heterogeneity aware: accommodates clients with different architectures.</li>
</ul>
<div class="fig mid">
<img src="fig16.png" alt="Figure 16 One-shot federated learning: client-side synthetic data plus server-side ensemble distillation">
<div class="cap"><span class="zh">图16 单轮通信联邦学习：客户端合成数据与服务器端集成蒸馏。</span><span class="en">Figure 16 One-shot federated learning: client-side synthetic data plus server-side ensemble distillation.</span></div>
</div>
</div>
<br>


<div class="sub">
<h3><span class="zh">生成式数据增强：探索超材料结构</span><span class="en">Generative Augmentation: Exploring Metamaterial Structures</span></h3>
<p class="zh">早期设计依赖人工专业经验与手动设计。超材料具有可编程几何结构，可通过设计几何结构定制特定功能；研究基于体素化表示构建几何候选体结构，并在生成过程中平衡合理性、新颖性与多样性。</p>
<p class="en">Early design relied on expert experience and manual effort. Metamaterials have programmable geometry, so specific functions can be tailored by designing that geometry. Candidates are built on voxelized representations, with generation balancing plausibility, novelty and diversity.</p>
<div class="fig mid">
<img src="fig17.png" alt="Figure 17 Metamaterial inverse design with a 3D conditional diffusion model and data augmentation">
<div class="cap"><span class="zh">图17 超材料逆向设计：3D 条件扩散模型与数据增强。</span><span class="en">Figure 17 Metamaterial inverse design with a 3D conditional diffusion model and data augmentation.</span></div>
</div>
</div>
</div>
<br>


<!-- summary -->
<div class="sec" id="summary">
<div class="sec-head"><span class="sec-no">05</span><h2><span class="zh">总结：从对抗样本到生成式数据增强</span><span class="en">Summary: From Adversarial Examples to Generative Data Augmentation</span></h2></div>
<p class="zh">两条路线共享同一套底层机制——学习数据空间中的有效扰动、利用高维空间的“线性敏感性”，最终都服务于模型的鲁棒性与泛化能力；差别在于扰动的目标与约束。</p>
<p class="en">Both routes share the same underlying mechanisms — learning effective perturbations in data space and exploiting the linear sensitivity of high-dimensional space — and both ultimately serve robustness and generalization. They differ in the objective and constraints placed on the perturbation.</p>
<table class="table">
<thead><tr><th><span class="zh">维度</span><span class="en">Dimension</span></th><th><span class="zh">对抗样本</span><span class="en">Adversarial examples</span></th><th><span class="zh">生成式数据增强</span><span class="en">Generative data augmentation</span></th></tr></thead>
<tbody>
<tr><td><span class="zh">扰动目标</span><span class="en">Perturbation goal</span></td><td><span class="zh">约束条件下的定向扰动生成，目标“破坏模型性能”</span><span class="en">Constrained, targeted perturbation aimed at breaking model performance</span></td><td><span class="zh">分布约束下的自然扰动生成，目标“保持语义、增加变化”</span><span class="en">Distribution-constrained, natural perturbation aimed at preserving semantics while adding variation</span></td></tr>
<tr><td><span class="zh">高维线性敏感性</span><span class="en">Linear sensitivity</span></td><td><span class="zh">定向累积扰动以实现错误分类</span><span class="en">Accumulating targeted perturbations to force misclassification</span></td><td><span class="zh">微小扰动不改变语义，仅增加多样性</span><span class="en">Small perturbations that leave semantics intact and add diversity</span></td></tr>
<tr><td><span class="zh">对模型的价值</span><span class="en">Value to the model</span></td><td><span class="zh">通过对抗训练暴露模型脆弱点，学会应对攻击（安全威胁）</span><span class="en">Adversarial training exposes vulnerabilities so the model learns to resist attacks (security threats)</span></td><td><span class="zh">通过补充训练数据覆盖更多场景，缓解数据稀缺与分布偏移</span><span class="en">Supplementary training data cover more scenarios, relieving data scarcity and distribution shift</span></td></tr>
</tbody>
</table>
<div class="note"><span class="zh">核心判断：模型能力上限取决于数据质量、结构与组织方式。对抗样本揭示了数据空间中“危险的方向”，生成式数据增强则把这些方向转化为“有用的多样性”。</span><span class="en">Core claim: a model’s capability ceiling is set by data quality, structure and organization. Adversarial examples reveal the dangerous directions in data space; generative data augmentation turns those directions into useful diversity.</span></div>
<p class="quote"><span class="zh">从对抗样本到生成式数据增强</span><span class="en">From adversarial examples to generative data augmentation</span></p>
</div>
</div>
<script>
(function () {
  var root = document.getElementById('r2');
  var btn = document.getElementById('toggle');
  if (!root || !btn) { return; }
  var stored = null;
  try { stored = window.localStorage.getItem('r2_lang'); } catch (e) { stored = null; }
  var param = null;
  try { param = new URLSearchParams(window.location.search).get('lang'); } catch (e) { param = null; }
  function apply(lang) {
    if (lang !== 'en') { lang = 'zh'; }
    root.classList.remove('lang-zh', 'lang-en');
    root.classList.add('lang-' + lang);
    btn.textContent = (lang === 'zh') ? 'EN' : '中文';
    btn.setAttribute('data-lang', lang);
    btn.setAttribute('title', (lang === 'zh') ? 'Switch to English' : '切换到中文');
    try { window.localStorage.setItem('r2_lang', lang); } catch (e) {}
  }
  btn.addEventListener('click', function () {
    apply(btn.getAttribute('data-lang') === 'zh' ? 'en' : 'zh');
  });
  apply(param || stored || 'zh');
})();
</script>
