---
# title: "An example conference paper"
title: "Diffusion Reconstruction-based Data Likelihood Estimation for Core-Set Selection"
authors:
- Mingyang Chen 
- Jiawei Du 
- Bo Huang 
- Yi Wang
- Xiaobo Zhang
- Wei Wang

date: ""
doi: "10.48550/arXiv.2511.19274"

# Schedule page publish date (NOT publication's date).
publishDate: "2025-11-24T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: In * AAAI Conference on Artificial Intelligence (AAAI'26).*
publication_short: In *AAAI2026*

abstract: Existing core-set selection methods predominantly rely on heuristic scoring signals such as training dynamics or model uncertainty, lacking explicit modeling of data likelihood. This omission may hinder the constructed subset from capturing subtle yet critical distributional structures that underpin effective model training. In this work, we propose a novel, theoretically grounded approach that leverages diffusion models to estimate data likelihood via reconstruction deviation induced by partial reverse denoising. Specifically, we establish a formal connection between reconstruction error and data likelihood, grounded in the Evidence Lower Bound (ELBO) of Markovian diffusion processes, thereby enabling a principled, distribution-aware scoring criterion for data selection. Complementarily, we introduce an efficient information-theoretic method to identify the optimal reconstruction timestep, ensuring that the deviation provides a reliable signal indicative of underlying data likelihood. Extensive experiments on ImageNet demonstrate that reconstruction deviation offers an effective scoring criterion, consistently outperforming existing baselines across selection ratios, and closely matching full-data training using only 50% of the data. Further analysis shows that the likelihood-informed nature of our score reveals informative insights in data selection, shedding light on the interplay between data distributional characteristics and model learning preferences.

# Summary. An optional shortened abstract.
# summary: We encouraging ensemble diversity on learning high-level feature representations and gradient dispersion in simultaneous training of deep ensemble networks.


# links:
url_pdf: https://arxiv.org/pdf/2511.19274
url_code: https://github.com/mchen725/DRD
# url_dataset: ''
# url_poster:  ''
# url_project: ''
# url_slides: ''
# url_source: ''
# url_video: ''
---
