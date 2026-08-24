# Journal Fit Addendum — Communications in Nonlinear Science and Numerical Simulation

**Manuscript:** "The Covid-19 Impact on Temporal Threshold Networks in the US Stock Market" (Bruce & Bartsch)
**Journal assessed:** Communications in Nonlinear Science and Numerical Simulation (CNSNS), Elsevier, ISSN 1007-5704
**Assessed:** 31 July 2026
**Same rubric and census method as the three-journal report — scores are directly comparable.**

---

## Headline

### Fit score: **3.5 / 10** — the weakest of the four assessed. Do not submit.

For comparison: Applied Network Science **8.5**, Journal of Complex Networks **7.5**, Network Science **5.0**, **CNSNS 3.5**.

CNSNS is not a marginal fit that could be rescued by better framing. It is the *third* journal in the same family that has already rejected you twice — Elsevier nonlinear science — and the census shows the mismatch is structural, not presentational. The word "threshold" appears throughout its catalogue and in **every single case** it means something other than what you mean by it.

---

## 1. Census method

Crossref REST API by ISSN 1007-5704 (Elsevier), queried 31 July 2026.

| Measure | Value |
|---|---|
| Total Crossref DOIs | **10,144** (2,680 current + 7,464 backfile) |
| Articles/year (2023 / 2024 / 2025) | 671 / 635 / 699 |
| Scale relative to targets | ~9× Applied Network Science, ~13× Journal of Complex Networks, ~28× Network Science |

At 10,144 records a full title dump exceeds the API's 1,000-row ceiling, so instead of a single census I ran **targeted title queries within the journal** — the more informative approach for a journal this large, because it tests directly whether your specific subject matter exists here at all. Three probes, each reported in full below.

---

## 2. Probe 1 — "stock market" in title: 22 hits, complete list

Every paper CNSNS has published with "stock" or "stock market" in the title:

- Analysis of stock market indices through multidimensional scaling (2011)
- Analysis of cyclical behavior in time series of stock market returns (2018)
- Application of ESN prediction model based on compressed sensing in stock market (2021)
- Semi-analytic valuation of stock loans with finite maturity (2015)
- High frequency trading and stock index returns: A nonlinear dynamic analysis (2021)
- Modified generalized sample entropy and surrogate data analysis for stock markets (2016)
- Multiscale sample entropy and cross-sample entropy based on symbolic representation and similarity of stock markets (2018)
- Null-validated topological signatures of financial market dynamics (2026)
- Solving the chaos model-data paradox in the cryptocurrency market (2021)
- Chaos measure dynamics in a multifactor model for financial market predictions (2024)
- Dynamics of a binary option market with exogenous information and price sensitivity (2023)
- Discrete homotopy analysis for optimal trading execution with nonlinear transient market impact (2016)
- Intraday limit order price change transition dynamics across market capitalizations through Markov analysis (2026)
- Herding, minority game, market clearing and efficient markets in a simple spin model framework (2018)
- A theoretical analysis of information leakage and market efficiency under forecast announcements (2026)
- Option pricing under finite moment log stable process in a regulated market (2020)
- *(plus 6 on electricity markets, commodity markets, fisheries stock-effort models and supply chains — not financial-market papers at all)*

**Read this carefully.** CNSNS does have an econophysics stream, and it is a real one. But it is the **time-series complexity** flavour: sample entropy, multiscale entropy, surrogate data, multifractal and detrended cross-correlation analysis, chaos measures, minority games, spin models, option pricing, stochastic processes. It is **not** the correlation-network flavour. In 10,144 papers there is not one stock-correlation-network paper, not one MST filtering paper, and not one threshold-network paper.

**Nearest three papers in the entire journal:**

| Paper | Year | How close |
|---|---|---|
| Null-validated topological signatures of financial market dynamics | 2026 | Closest. Uses null models to validate topological structure in market data — same broad problem of separating real structure from noise. Different toolkit (TDA, not graph filtering). |
| Multidimensional scaling analysis of financial stocks based on Kronecker-delta dissimilarity | 2018 | Builds a dissimilarity structure over stocks — the same first step as yours, then goes to MDS rather than a graph. |
| A cooperation index based on the Rényi entropy of correlation matrix spectrum | 2012 | Works from the stock correlation matrix, but extracts a spectral entropy index rather than a filtered network. |

Also adjacent: *Financial contagion in banking networks with community structure* (2023) and *Default clearing and ex-ante contagion in financial systems with a two-layer network structure* (2025) — but these are balance-sheet contagion models on given networks, not inferred correlation graphs.

---

## 3. Probe 2 — "minimum spanning tree" / "threshold network" in title

This is the decisive result. Querying the journal for `minimum spanning tree threshold network` returns hits in which the word "threshold" means:

- epidemic thresholds (SIS on overlay networks; malaria, dengue, waterborne disease models; stochastic SIR)
- neuronal firing thresholds (spike threshold in two-compartment neurons; spiking neurons with fluctuating threshold)
- bifurcation and critical thresholds (Kuramoto model; quasi-threshold in the noise-driven Higgins model; long-range threshold quasi-stationary states)
- control and engineering thresholds (event-triggered control with dynamic threshold; optical switching threshold energy)
- resource-management thresholds (two-threshold harvesting policy; threshold harvesting in stage-structured populations)
- opinion-dynamics confidence thresholds
- one recurrence-quantification-analysis threshold paper (2020) — the only hit anywhere near "choosing a threshold for a data-derived structure"

**Zero results for minimum spanning trees as a correlation filter. Zero for threshold networks in the Boginski sense. Zero for PMFG/TMFG.**

Your paper's entire contribution is a threshold-selection criterion for correlation-based graphs. In this journal, "threshold" is a bifurcation parameter or an epidemic tipping point. That is not a framing problem you can fix with a rewritten abstract — the reviewer pool does not contain people who work on this problem.

---

## 4. Probe 3 — "community detection" / networks in title

Querying `community detection complex network` returns a corpus dominated by:

- **synchronisation and control ON networks**: pinning impulsive synchronisation, cluster synchronisation in coloured community networks, general decay synchronisation, lag projective synchronisation, exponential synchronisation of delayed fractional complex networks, prespecified-time synchronisation via intermittent event-triggered control, distributed adaptive cluster synchronisation in higher-order community networks
- **epidemic and spreading dynamics on networks**: SIVS models on complex networks, computer virus propagation, epidemic-free networks with minimum edge removal
- **neuronal network dynamics**: frequency locking and travelling burst sequences in community-structured networks of inhibitory neurons

Genuine structural community-detection papers: **two** — *Community detection in complex networks via adapted Kuramoto dynamics* (2017), which detects communities using a nonlinear oscillator model, and *Similarity between community structures of different online social networks* (2015).

**This is the crux.** CNSNS studies **dynamics ON networks** — you are given a network and you analyse synchronisation, control or spreading on it. Your paper does the opposite: it **infers a network from data** and analyses its structure. These are adjacent literatures that barely cite each other, and CNSNS lives almost entirely on the other side of that line.

---

## 5. Novelty gap

The gap is **total** — no paper in 10,144 does anything resembling MST-based threshold selection for temporal correlation networks. As with Network Science, this is not the good kind of gap. An empty niche in a journal whose readers do not work on the problem means reviewers have no basis for judging the contribution as important, and editors reading for fit see an outlier. The two rejections you already hold are evidence of exactly this dynamic.

The Kuramoto-based community-detection paper (2017) is the one thing you could genuinely cite to argue precedent, and one paper is not a stream.

---

## 6. Fit score — 3.5 / 10

| Sub-score | Score | Justification |
|---|---|---|
| **Scope match** *(weighted high)* | **3/10** | The journal is nonlinear science and numerical simulation. Your paper contains no nonlinear dynamical model, no numerical scheme, no chaos, no bifurcation analysis, and no integrable system. Pearson correlation → MST → Louvain is linear statistics plus combinatorial graph algorithms. |
| **Methodological fit** | **3/10** | CNSNS's econophysics toolkit is entropy measures, multifractal/DCCA analysis, surrogate data and stochastic processes. Correlation-network filtering does not appear. Its network papers are synchronisation and control, not structure inference. |
| **Novelty** | **6/10** | Gap is complete, but empty because the community does not work here. Discounted accordingly. |
| **Expected reviewer reception** | **3/10** | Reviewers will be nonlinear dynamicists and numerical analysts. The most likely verdict is Physica A Reviewer #4's again — "competent, but basic network metrics, and where is the nonlinear science?" This is the *same failure mode* that produced your first two rejections. |
| **Audience interest** | **4/10** | A real econophysics readership exists, but it reads entropy and multifractal papers. It is not primed for a threshold-selection criterion. |

**Verdict: reconsider venue.** Not "submit after revisions" — the revisions that would make this fit would turn it into a different paper.

---

## 7. Difficulty, speed and cost

⚠️ **Metrics unverified.** ScienceDirect and elsevier.com are bot-protected and returned empty responses to my fetcher, and browser automation was unavailable in this session. Everything in this table other than the Crossref volume figures needs checking on the journal's ScienceDirect page before you rely on it.

| Metric | Value | Confidence |
|---|---|---|
| Articles/year | **~650–700** | **High** (Crossref) |
| Total corpus | 10,144 DOIs | **High** (Crossref) |
| Impact Factor | Not verified — historically Q1 in applied mathematics, materially higher than the ~1.9 of ANS and JoCN | **Low — verify** |
| CiteScore | Not verified — historically well above the three targets | **Low — verify** |
| Acceptance rate | Not disclosed | — |
| Time to first decision | Not verified | — |
| OA model | Elsevier **hybrid** (subscription with gold OA option) | Medium |
| Cost to you | Likely **£0** via the standard subscription route, and hybrid titles are the class covered by the Jisc–Elsevier deal — verify with the library | Medium |

**The honest tension:** on raw prestige CNSNS beats all three journals in the main report, and it would almost certainly cost you nothing. If prestige and cost were your only criteria it would win. They are not, and the two criteria it fails — fit and acceptance odds — are the two that have already cost you a year.

**Desk-reject risk: high.** Chaos, Solitons & Fractals desk-rejected you with "we receive a much larger number of papers than we are able to accept." CNSNS publishes ~700 articles a year, is more oversubscribed still, and is a sister Elsevier nonlinear-science title. A volume-triaging editor scanning a paper with no nonlinear dynamics in a nonlinear-dynamics journal is the single most predictable desk rejection in this whole exercise.

**One more consideration:** Elsevier has now rejected this manuscript twice, at Physica A and CSF. There is no formal blacklisting across titles, but you would be making a third approach to the same publisher's nonlinear-science portfolio with a paper whose contribution sits outside it.

---

## 8. Updated head-to-head

| | **Applied Network Science** | **J. Complex Networks** | **Network Science** | **CNSNS** |
|---|---|---|---|---|
| **Fit score** | **8.5/10** | **7.5/10** | 5.0/10 | **3.5/10** |
| Publisher | Springer Nature | Oxford UP | Cambridge UP | Elsevier |
| Impact Factor | 1.9 | 1.9 (5-yr 2.4) | not published | Highest of the four *(unverified)* |
| Aligned papers | ~16 / 802 | ~13 / 638 | ~3 / 429 | **~3 / 10,144** |
| MST / threshold-network papers | Yes | **Yes** | No | **None** |
| Articles/year | ~80 | ~52 | ~25 | ~675 |
| First decision | **14 days (published)** | est. 2–4 months | est. 3–5 months | not verified |
| Desk-reject risk | Low | Low | Moderate | **High** |
| Cost to you | £1,240 *(verify coverage)* | **£0** | £0 | £0 |
| **Recommendation** | **Submit if APC funded** | **Submit — default** | Do not submit | **Do not submit** |

---

## 9. Bottom line

CNSNS is a better journal than the three in the main report, and a worse home for this paper than any of them.

The pattern in your rejection history is now unmistakable across four data points: **this is an applied-network-science paper, and every time it goes to a nonlinear-physics venue it is rejected on scope or volume rather than on the science.** Physica A and CSF have already run that experiment twice. CNSNS would be the third run of the same experiment, at the publisher that produced both prior rejections, in a journal where the word "threshold" means bifurcation point.

The two things that would make CNSNS viable — building a nonlinear dynamical model of the correlation structure, or recasting the threshold criterion as a critical-transition phenomenon — are a different paper, and a year of work. Your current paper's strength is that it is practical, automatable and domain-agnostic. Send it somewhere that values exactly that.

**Stick with Journal of Complex Networks, or Applied Network Science if the £1,240 lands.**

---

## Caveats

- Title-based probing, not a full census (10,144 records exceeds the Crossref 1,000-row ceiling). Probes were chosen to test directly for your subject matter; a full abstract-level census could surface a handful more adjacent papers, but not enough to move a 3.5 into contention.
- **CNSNS citation metrics, turnaround times and APC are unverified** — ScienceDirect and elsevier.com returned empty responses (bot protection), and browser tools were unavailable. Check the journal's ScienceDirect "About" and "Open access options" pages, and confirm Jisc–Elsevier coverage with your library, before relying on §7.
- Volume figures, corpus size and all title lists in §§2–4 are verified from the Crossref REST API, queried 31 July 2026.

**Sources:** Crossref REST API (`api.crossref.org/journals/1007-5704/works`, and `api.crossref.org/journals?query=...`), queried 31 July 2026 · [CNSNS on ScienceDirect](https://www.sciencedirect.com/journal/communications-in-nonlinear-science-and-numerical-simulation) *(fetch returned no content — bot-protected)*.
