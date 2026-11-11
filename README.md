## Jeremy D. Wu

Mathematician by training. My PhD is in probability theory at the University of Pennsylvania, with a
master's in statistics from Wharton taken alongside it. I publish across causal inference and
econometric methods, machine learning and language models, and probability theory, and I build the
data pipelines and test harnesses that work of that kind needs.

[dwuuuuuu.github.io](https://dwuuuuuu.github.io) &nbsp;·&nbsp; [Google Scholar](https://scholar.google.com/citations?user=RGvMvRIAAAAJ&hl=en) &nbsp;·&nbsp; [LinkedIn](https://www.linkedin.com/in/jeremydwu)

### Work here

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

### How I work

Claude Code and Codex are my primary development workflow, for research code, data pipelines and
test suites. Verification is the part I own: property-based tests rather than output snapshots, and
an audit stage that re-reads model output against the source. One test in the harness multiplies all
future prices by five and requires earlier results to be bit-identical.
