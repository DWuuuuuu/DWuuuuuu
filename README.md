## Jeremy D. Wu

I am an interdisciplinary researcher. My PhD is in probability theory at the University of
Pennsylvania, with a master's in statistics from Wharton taken alongside it, and my published work
runs across four fields that are usually four different people:

- **Machine learning, language models and evaluation.** Post-training and preference
  optimization, multimodal and vision-language models, and measuring where model reasoning breaks.
- **Causal inference.** Observational study design with multiple control groups, familywise error
  control, and sensitivity analysis for unmeasured confounding.
- **Econometrics and quantitative research.** Hedonic and panel identification at scale, LLM and
  NLP measurement of unstructured data, and the point-in-time discipline strategy research needs.
- **Probability theory.** Random contingency tables, asymptotic enumeration, and SLE.

Reviewer for NeurIPS, ICML, ICLR and PNAS.

[dwuuuuuu.github.io](https://dwuuuuuu.github.io) &nbsp;·&nbsp; [Google Scholar](https://scholar.google.com/citations?user=RGvMvRIAAAAJ&hl=en) &nbsp;·&nbsp; [LinkedIn](https://www.linkedin.com/in/jeremydwu)

### Machine learning, language models and evaluation

**[GestaltMML](https://github.com/WGLab/GestaltMML)**

A vision-language model for rare disease diagnosis, and the first multimodal framework to combine
facial images with clinical text. Top-1 accuracy of 50.1% against 43.0% for the strongest published
image-only baseline, on a 528-disorder benchmark, and better on all four reported metrics. I am the
only contributor to the repository.

*Paper.* **[GestaltMML: enhancing rare genetic disease diagnosis through multimodal machine learning
combining facial images and clinical text](https://arxiv.org/abs/2312.15320).**
**Wu, D.**, Wang, Z., Chen, H. et al. IEEE BIBM 2026, accepted. 14 pages.

**[MINT-LLM](https://github.com/WGLab/MINT-LLM)**

Reinforcement learning with odds-ratio preference optimization, aligning language models of 3B to
11B parameters. The preference signal came from GestaltMML rather than from human annotators,
because the records are access-restricted and qualified annotators for them are scarce.

*That constraint shaped the design more than any hyperparameter did.*

*Paper.* **[Multimodal integrated knowledge transfer to large language models through preference
optimization](https://doi.org/10.1016/j.patter.2026.101544).**
Wang, Z.†, **Wu, D.**†, Nguyen, Q.M., Xu, Z., Wang, K. *Patterns* 7(8), 101544 (2026).
ICML 2025 GenBio Workshop spotlight. †Joint first authors.

**[PhenoGPT](https://github.com/WGLab/PhenoGPT)**

Phenotype recognition from clinical notes, and the most used of these three repositories.

*Paper.* **[Enhancing phenotype recognition in clinical notes using large language
models](https://doi.org/10.1016/j.patter.2023.100887).**
Yang, J., Liu, C., Deng, W., **Wu, D.**, Weng, C., Zhou, Y., Wang, K. *Patterns* 5(1) (2024).
32 pages in the preprint.

**[CoT-RAG-LLM-Gene-Prioritization-Disease-Diagnosis](https://github.com/WGLab/CoT-RAG-LLM-Gene-Prioritization-Disease-Diagnosis)**

Chain-of-thought prompting with retrieval-augmented generation for rare disease diagnosis and gene
prioritization, across five inference methods, with FAISS retrieval over biomedical embeddings,
reranking, and an automated evaluator. I am a contributor to the repository and joint first author
on the paper.

*Paper.* **[Integrating chain-of-thought and retrieval-augmented generation enhances rare disease
diagnosis from clinical notes](https://doi.org/10.1002/mdb2.70033).**
Wang, Z.†, **Wu, D.**†, Nguyen, Q., Wang, K. *Medicine Bulletin* 2(2), 167–183 (2026).
17 pages. †Joint first authors.

Further papers in this area:

- **[Exploring the reversal curse and other deductive logical reasoning in BERT- and GPT-based large
  language models](https://doi.org/10.1016/j.patter.2024.101030).**

  **Wu, D.**†, Yang, J.†, Wang, K. *Patterns* 5(9), 101030 (2024). 26 pages in the preprint.
  †Joint first authors.

  *An evaluation study: the artifact is the design, not the code.*
- **[Classification of integers based on residue classes via modern deep learning
  algorithms](https://doi.org/10.1016/j.patter.2023.100860).**

  **Wu, D.**, Yang, J., Ahsan, M.U., Wang, K. *Patterns* 4(12) (2023). 14 pages in the preprint.
- **[Interpretable fine-tuned large language models facilitate making genetic test decisions for
  rare diseases](https://doi.org/10.1038/s41746-026-02733-z).**

  Nguyen, Q.M., Chen, F., Liu, C., Campbell, I.M., Zhang, G., **Wu, D.** et al.
  *npj Digital Medicine* (2026). 15 pages.

### Causal inference

- **Three-sided testing with two control groups, with an application to an observational study of
  the impact of high school football participation on subsequent cognitive functioning.**

  **Wu, D.**†, Horng, I.†, Deshpande, S.,
  [Small, D.](https://statistics.wharton.upenn.edu/profile/dsmall/) Preprint. †Joint first authors.

  *The procedure controls the familywise error rate across two control groups and bounds
  sensitivity to unmeasured confounding, which is what it takes to say anything credible about
  longitudinal cognitive decline when nobody can randomise who plays football.*
- **[Characterizing autism phenotype onset in the electronic health records to enable age-specific
  screening](https://doi.org/10.1002/aur.70378).**

  Chen, F., Kneifati-Hayek, J., Zelin, C., **Wu, D.** et al. *Autism Research* (2026).

  *Timing of phenotype onset across longitudinal records, which is what makes age-specific
  screening possible rather than a single prevalence figure.*

At CHOP I also built the evaluation pipelines for multimodal and longitudinal clinical data that
work of this kind depends on.

### Econometrics and quantitative research

**Green alpha in commercial real estate.**
Head of Quantitative Research at Mina Analytics, and co-author with Chief Economist
[Charles W. Calomiris](https://en.wikipedia.org/wiki/Charles_Calomiris) of the Real Estate Model.
I built the AI and NLP measurement layer and the identification strategy, and supervised junior
researchers across data engineering, feature construction and pipelines.

- **The question.** Not whether certified buildings rent for more, which is a selection artifact,
  but the **green premium** itself: what LEED or Energy Star certification adds to lease revenue
  per square foot for a given building, in a given location, in a given year. A single average is
  the wrong object. The premium is a surface over location and time, and estimating it at that
  resolution is what the model is for.
- **Data.** 36,000+ building-year observations across 1,322 zip codes in California and Florida,
  assembled from 10,000 datasets and ten terabytes. Unbalanced panels, 2015 to 2023 for California
  and 2017 to 2023 for Florida, roughly 22% Class A, 60% B, 17% C.
- **LLM extraction.** Broker brochures and listing text read into hard indicators, gym, rooftop
  deck, ocean view, by an LLM under targeted prompt engineering, validated to close to 100%
  accuracy against hand-coded text before the variables were allowed into the model.
- **NLP for what the LLM cannot binarise.** An LDA topic model turns the same corpus into
  per-building topic weights that come out interpretable as accessibility or quality of finishes,
  alongside tone, description length and word novelty. These are the variables that let a hedonic
  model see a view or a facade, which no traditional vendor carries.
- **Identification.** A hedonic specification that estimates a full baseline first, with no
  certification term in it, and only then adds certification and its interactions. Certification is
  positively selected, so conditioning on the whole baseline before the treatment makes the
  estimate deliberately conservative. The trap it avoids: new buildings are both likelier to be
  certified and worth more per square foot, so a model without age attributes vintage to green,
  which is the error published elsewhere in the industry.
- **Variable selection and validation.** Roughly 4,900 locational and 100 building-level candidates
  compete by forward selection on two criteria, incremental R squared and then significance at 1%,
  so a variable that matters but barely varies can still enter. Continuous variables trimmed at the
  5th and 95th percentiles; 9-fold cross-validation selecting on 80% and scoring on the held-out
  20%; variables surviving 7 of the other 8 folds added back. Final baselines: 881 variables in
  California, 709 in Florida, adjusted R squared 0.713 and 0.615.
- **Ruling out the obvious alternative.** If the premium were landlords recovering energy savings
  rather than tenants paying for green, lease type would order the effect. It does not: the triple
  net interaction comes in at 0.30 against 0.39 where the tenant pays nothing, which is backwards
  for cost pass-through, and the lease-type variables are not selected at all in Florida.
- **Results.** Average LEED premium of **8.3%** in California and **3.9%** in Florida, Energy Star
  **7.7%** and **7.3%**. The same model with no interactions gives 6.1% and 5.9% for LEED, so a
  single flat coefficient understates California and overstates Florida at the same time. The
  heterogeneity is the finding, not a caveat to it.
- **Down to one building.** Two uncertified towers in the same downtown Los Angeles zip code.
  Certifying one is worth 12% more lease revenue per square foot, about **$780K a year**.
  Certifying the other is worth nothing.

Findings were presented to institutional investors and to the U.S. Securities and Exchange
Commission.

*Paper.* **Estimating value creation in commercial real estate from green certification.**
Calomiris, C.W. and **Wu, J.** Working paper, November 2025. 31 pages.

**[investment-research-engine](https://github.com/DWuuuuuu/investment-research-engine)**

My personal quantamental research engine: cross-market screening for US and A-share equities,
fundamental valuation, macro and policy-path state, and public prediction markets, in one workflow.
47 modules, 258 tests.

*Point-in-time archiving, so that nothing I test can see data it would not have had.*

**[Epigram](https://epi-gram.app)**

A quantitative finance interview preparation platform, which I run as Head of Product, with two Ivy
League master's programs as institutional customers.

I own the corpus: roughly 300 probability, statistics and quantitative-reasoning problems of the
kind quant interviews actually ask, each with multiple verified solution paths. It doubles as an
evaluation set for reasoning models, which is why evaluation is not only a research interest for
me. I assign the difficulty, topic, reasoning-type and source-company labels myself, *because a
label a model assigns to its own output is not evidence.*

The code is at [chkim15/epigram](https://github.com/chkim15/epigram), my co-founder's repository,
and I commit to it there.

### Probability theory

Four sole-authored papers, from the PhD and just after it.

- **[On properties of random binary contingency tables with non-uniform
  margin](https://doi.org/10.30757/alea.v20-51).**

  *ALEA, Lat. Am. J. Probab. Math. Stat.* 20, 1367–1383 (2023). 17 pages.

- **[Asymptotic properties of random contingency tables with uniform
  margin](https://doi.org/10.1007/s10959-022-01234-5).**

  *Journal of Theoretical Probability* 36, 2066–2092 (2023). 27 pages.

- **[Asymptotic enumeration of binary contingency tables and comparison with the independence
  heuristic](https://doi.org/10.47443/cm.2023.037).**

  *Contributions to Mathematics* 8, 16–23 (2023). 8 pages.

- **[The SLE bubble measure via conformal welding of quantum
  surfaces](https://arxiv.org/abs/2302.13992).**

  PhD thesis, University of Pennsylvania (2023). 49 pages.

### How I work

Claude Code and Codex are my primary development workflow, for research code, data pipelines and
test suites. Verification is the part I own: property-based tests rather than output snapshots, and
an audit stage that re-reads model output against the source.

*One test in my backtesting code multiplies all future prices by five and requires earlier results
to be bit-identical.*

Source of the personal site is in [DWuuuuuu.github.io](https://github.com/DWuuuuuu/DWuuuuuu.github.io).
