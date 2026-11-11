## Jeremy D. Wu

Mathematician by training. My PhD is in probability theory at the University of Pennsylvania, with a
master's in statistics from Wharton taken alongside it. I publish across causal inference and
econometric methods, machine learning and language models, and probability theory, and I build the
data pipelines and test harnesses that work of that kind needs.

[dwuuuuuu.github.io](https://dwuuuuuu.github.io) &nbsp;·&nbsp; [Google Scholar](https://scholar.google.com/citations?user=RGvMvRIAAAAJ&hl=en) &nbsp;·&nbsp; [LinkedIn](https://www.linkedin.com/in/jeremydwu)

### Work here

**[epigram](https://github.com/chkim15/epigram)**
The product I run as Head of Product: a math learning platform, Next.js on Supabase and Postgres,
with two Ivy League master's programs as institutional customers. I own the problem corpus, every
solution path in it verified by hand. The repo lives on my co-founder Chulhee Kim's account and I
commit to it there.

**[quant-research-harness](https://github.com/DWuuuuuu/quant-research-harness)**
Backtesting engine for long-only cross-sectional equity strategies. Point-in-time data discipline,
explicit transaction and tax costs, and 51 tests, one of which asserts that future prices cannot
change past decisions. It ships a study that failed rather than dropping it.

**[investment-research-engine](https://github.com/DWuuuuuu/investment-research-engine)**
The research terminal around that engine: cross-market screening for US and A-share equities,
valuation, macro and policy-path state, and public prediction markets, in one workflow. 47 modules,
258 tests.

**[DWuuuuuu.github.io](https://github.com/DWuuuuuu/DWuuuuuu.github.io)**
Source of the personal site.

### Research code

Code for the papers, in the Wang Genomics Lab organisation at CHOP and Penn.

**[GestaltMML](https://github.com/WGLab/GestaltMML)**
The first multimodal framework for rare disease diagnosis to combine facial images with clinical
text. My first-author paper, and I am the only contributor to the repository.

**[MINT-LLM](https://github.com/WGLab/MINT-LLM)**
Multimodal knowledge transfer into language models through preference optimization. Co-authored with
Zhanliang Wang; published in Patterns, spotlight at the ICML 2025 GenBio workshop.

**[PhenoGPT](https://github.com/WGLab/PhenoGPT)**
Phenotype recognition from clinical notes. Co-authored, and the most used of these: 34 stars.

### How I work

Claude Code and Codex are my primary development workflow, for research code, data pipelines and
test suites. Verification is the part I own: property-based tests rather than output snapshots, and
an audit stage that re-reads model output against the source. One test in the harness multiplies all
future prices by five and requires earlier results to be bit-identical.
