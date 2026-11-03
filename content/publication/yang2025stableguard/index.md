---
# title: "An example conference paper"
title: "StableGuard: Towards Unified Copyright Protection and Tamper Localization in Latent Diffusion Models"
authors:
- Haoxin Yang
- Bangzhen Liu
- Xuemiao Xu 
- Cheng Xu
- Yuyang Yu
- Zikai Huang 
- Yi Wang
- Shengfeng He

date: ""
doi: "10.48550/arXiv.2509.17993"

# Schedule page publish date (NOT publication's date).
publishDate: "2025-09-22T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: In * Annual Conference on Neural Information Processing Systems (NeurIPS'25).*
publication_short: In *NeurIPS2025*

abstract: The advancement of diffusion models has enhanced the realism of AI-generated content but also raised concerns about misuse, necessitating robust copyright protection and tampering localization. Although recent methods have made progress toward unified solutions, their reliance on post hoc processing introduces considerable application inconvenience and compromises forensic reliability. We propose StableGuard, a novel framework that seamlessly integrates a binary watermark into the diffusion generation process, ensuring copyright protection and tampering localization in Latent Diffusion Models through an end-to-end design. We develop a Multiplexing Watermark VAE (MPW-VAE) by equipping a pretrained Variational Autoencoder (VAE) with a lightweight latent residual-based adapter, enabling the generation of paired watermarked and watermark-free images. These pairs, fused via random masks, create a diverse dataset for training a tampering-agnostic forensic network. To further enhance forensic synergy, we introduce a Mixture-of-Experts Guided Forensic Network (MoE-GFN) that dynamically integrates holistic watermark patterns, local tampering traces, and frequency-domain cues for precise watermark verification and tampered region detection. The MPW-VAE and MoE-GFN are jointly optimized in a self-supervised, end-to-end manner, fostering a reciprocal training between watermark embedding and forensic accuracy. Extensive experiments demonstrate that StableGuard consistently outperforms state-of-the-art methods in image fidelity, watermark verification, and tampering localization.

# Summary. An optional shortened abstract.
# summary: We encouraging ensemble diversity on learning high-level feature representations and gradient dispersion in simultaneous training of deep ensemble networks.


# links:
url_pdf: https://arxiv.org/pdf/2509.17993
url_code: https://github.com/Harxis/StableGuard
# url_code: ''
# url_dataset: ''
# url_poster:  ''
# url_project: ''
# url_slides: ''
# url_source: ''
# url_video: ''
---
