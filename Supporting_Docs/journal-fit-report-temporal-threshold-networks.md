# Journal Fit Assessment — Three-Way Comparison

**Manuscript:** "The Covid-19 Impact on Temporal Threshold Networks in the US Stock Market"
**Authors:** Christopher Michael Bruce & Thomas Bartsch (Dept of Mathematical Sciences / Centre for Nonlinear Mathematics and Applications, Loughborough University)
**Assessed:** 31 July 2026
**Journals assessed:** Applied Network Science (Springer, fully OA) · Network Science (CUP) · Journal of Complex Networks (OUP)

---

## 0. Headline verdict

**Submit to the Journal of Complex Networks (OUP).**

Your instinct is half right and half wrong, and the half that's wrong is the expensive half.

- **You are right to prefer Applied Network Science on fit** — it is the best pure fit of the three (8.5/10) and has a *published* 14-day median to first decision, which is exceptional. If the £1,240 gets funded, go there.
- **You are wrong to lump Journal of Complex Networks in with Network Science.** JoCN is a genuinely good fit (7.5/10). It has a live econophysics/financial-correlation-network stream *and* a live temporal-networks stream, an IF and CiteScore matching or beating ANS, and it's **hybrid**, which is exactly the class of journal UK read-and-publish deals cover. You get ~90% of the ANS fit for £0.
- **You are right about Network Science, more so than you realise.** It is not a marginal fit, it is the wrong community (5/10). Its centre of gravity is social networks and statistical network modelling (ERGM, SAOM, blockmodels), and its scope explicitly asks for "rigorous theory building." In 429 papers across 13 years it has published essentially **three** finance papers and not one MST or threshold-filtering paper on market data. Drop it.

**The ranked plan:** JoCN first (or ANS first *if and only if* the APC is confirmed funded before you submit). Network Science is a distant third and I would not use it at all.

**On alternatives:** no venue I examined clearly beats ANS or JoCN on your combined criteria. Two are worth holding in reserve — *Journal of Physics: Complexity* (IOP, good topical fit, check the IOP UK deal) and *Journal of Economic Interaction and Coordination* (Springer, **hybrid** so likely free to you, explicitly econophysics-friendly). See §7.

---

## 1. Method and reproducibility of the census

Complete back-catalogue censuses were run via the **Crossref REST API by ISSN**, retrieving all deposited records for each journal (no sampling):

| Journal | ISSN queried | Total Crossref records | Records since 2023-01-01 | Approx. articles/year |
|---|---|---|---|---|
| Applied Network Science | 2364-8228 | **802** | 286 | ~80 |
| Journal of Complex Networks | 2051-1329 | **638** | 187 | ~52 |
| Network Science | 2050-1250 | **429** | 88 | ~25 |

Query form: `https://api.crossref.org/journals/{ISSN}/works?rows=1000&select=title,DOI,published&sort=published&order=desc`. Because each total was under the 1,000-row ceiling, **each census is complete, not a sample.**

Tiering keyword set (case-insensitive, applied to titles): `stock · financ · market · correlation · spanning tree · econophys · threshold · systemic · portfolio · asset · trading · crypto · bank · temporal · time-varying · dynamic network · community detection · modularity · econom`.

**Caveats stated up front:** tiering is title-based, so expect ±3–4 papers of slippage in each tier; Crossref totals include editorials, corrections and front matter, so the "articles/year" figures are slight over-counts; Network Science's citation metrics are not published on its CUP journal page and are flagged as unverified below.

---

## 2. Applied Network Science (Springer Nature, ISSN 2364-8228)

### 2.1 Alignment table

| Tier | Count | Share of 802 |
|---|---|---|
| **Heavily aligned** (financial/market networks, correlation filtering, crisis-via-networks) | **~16** | ~2.0% |
| **Medium aligned** (temporal/dynamic networks, community detection, systemic-risk indicators, economic networks) | **~70** | ~8.7% |
| Low aligned (shared toolkit, unrelated domain) | remainder | — |

**Heavily aligned papers (complete list from the census):**

- Cross-validation of correlation networks using modular structure ⚠️ **novelty threat — cite this**
- Threshold sensitivity of the production network topology ⚠️ **thresholding, cite this**
- Network-based diversification of stock and cryptocurrency portfolios
- Spotting the stock and crypto markets' rings of fire: measuring change proximities among spillover dependencies within inter and intra-market asset classes
- Characterizing financial markets from the event driven perspective
- Graph learning on financial networks from pairwise similarity of firm-level characteristics
- Enhancing financial crisis prediction: integrating change point detection for exogenous event identification
- A multi-scale network framework in digital asset markets based on high-order information dynamics
- Signed network models for dimensionality reduction of portfolio optimization
- Signature-based portfolio allocation: a network approach
- Derivative trading networks: a spectral model for risk identification
- Default robustness and worst-case losses in financial networks
- FlowSeries: flow analysis on financial networks
- The multiplex nature of global financial contagions
- A network analysis of the non-fungible token (NFT) market: structural characteristics, evolution, and interactions
- Regionalization and continuing globalization scenarios as a result of re-globalization: … multiplex financial network
- Weirdnodes: centrality based anomaly detection on temporal networks for the anti-financial crime domain

**Representative medium-aligned (there are ~70; these show the temporal-networks depth):** Detection of dynamic communities in temporal networks with sparse data · Short- and long-term temporal network prediction based on network memory · Exploring temporal community evolution: algorithmic approaches and parallel optimization for dynamic community detection · Correlation networks of air particulate matter (PM₂.₅): a comparative study · Centrality measure and visualization technique for multiple-parent nodes of earthquakes based on correlation-metric.

**Read this:** ANS runs *both* streams your paper sits across — an active financial-networks stream and a deep temporal-networks/dynamic-community-detection stream. No other journal of the three has both at this depth. Note especially the PM₂.₅ and earthquake correlation-network papers: ANS publishes correlation networks built from *any* time series, which is precisely the audience for a domain-agnostic threshold criterion.

### 2.2 Fit score — **8.5 / 10**

| Sub-score | Score | Justification |
|---|---|---|
| Scope match | 9/10 | Scope states it "emphasizes on articles with direct applications to real-world problems" and "encompasses all fields that benefit from quantitative network-based modeling." Your paper is definitionally in scope. |
| Methodological fit | 8/10 | Correlation → MST → threshold → Louvain is standard currency here. No theorem required, which is the whole point. |
| Novelty | 7/10 | Gap holds (§5), but "Cross-validation of correlation networks using modular structure" and "Threshold sensitivity of the production network topology" are adjacent and *must* be engaged with, or a reviewer will say the gap isn't real. |
| Expected reviewer reception | 8/10 | Applied reviewers will value the automatability and the 2,456-stock scale. They will probe threshold sensitivity and the power-law claim — both of which you have already addressed. |
| Audience interest | 9/10 | Broadest, most applied readership of the three. 787.7k downloads in 2025. |

**Verdict: submit.** Lead with the criterion, use Covid-19 as the demonstration.

### 2.3 Difficulty & speed

| Metric | Value | Source |
|---|---|---|
| Journal Impact Factor (2025) | **1.9** | Springer journal page |
| 5-year JIF (2025) | **2.2** | Springer journal page |
| Submission → first decision (median) | **14 days** ✅ | Springer journal page (publisher-published) |
| Articles/year | ~80 | Crossref |
| Acceptance rate | Not disclosed | — |
| Indexing | Scopus, ESCI, DOAJ, DBLP, EI Compendex, INSPEC | Springer journal page |
| APC | **£1,240 / $1,790 / €1,490** + VAT | Springer "How to publish with us" |

**14 days to first decision is the single strongest speed number of the three, and it is a published figure rather than an estimate.** Combined with immediate OA publication on acceptance, ANS is almost certainly the fastest route to a citable DOI. Realistic trajectory: low desk-reject risk, minor-to-major revisions, plausible acceptance inside 3–4 months.

**Open collections (a gentler, topic-matched route in):**

| Collection | Deadline | Applicable? |
|---|---|---|
| Special Issue of the 14th Int'l Conference on Complex Networks and their Applications | **31 July 2026 — today** | Only if you presented at CN2025. Almost certainly not available. |
| Selected Contributions from the Int'l Symposium on Complex Systems 2026 | 3 October 2026 | Conference-linked; not applicable unless you attend. |
| Networks for everyday life | 30 November 2026 | Open, thematic — possible but a stretch for a finance paper. |

Conclusion: submit to the **general track**, not a collection.

### 2.4 What a sharp ANS reviewer will most probe

1. **"Why is the MST max edge weight the *right* threshold, not just *a* connected one?"** You have Figs 2–4 (components, edge %, modularity vs threshold) plus the out-of-sample post-Oct-2021 check. Put that argument in the abstract, not section II.
2. **"Have you compared against the alternatives on the same data?"** Xu et al.'s global threshold and Ku et al.'s MST-union construction are discussed but not benchmarked. A single comparison figure would close this.

---

## 3. Journal of Complex Networks (OUP, ISSN 2051-1329)

### 3.1 Alignment table

| Tier | Count | Share of 638 |
|---|---|---|
| **Heavily aligned** | **~13** | ~2.0% |
| **Medium aligned** (temporal/dynamic networks, community detection, systemic risk, economic networks) | **~48** | ~7.5% |
| Low aligned | remainder | — |

**Heavily aligned papers (complete list from the census):**

- **The origin of return correlation networks** ⚠️ **closest paper in any of the three journals — you must cite and differentiate from this**
- **Testing the randomness of correlation networks from multivariate time series** ⚠️ **direct competing threshold philosophy (significance filtering) — cite**
- Pearson correlations on complex networks
- An efficient algorithm to find all minimum spanning trees
- Analyzing communicability and connectivity in the Indian stock market during crises
- Risk-dependent centrality in the Brazilian stock market
- Extremal dependence networks for mitigating systemic risk via maximum independent sets
- Vector autoregression in cryptocurrency markets: unraveling complex causal networks
- VAR(1) long memory from bottlenecks and long cycles in network dynamics
- Markets as ecological networks: inferring interactions and identifying communities
- Systemic risk and structural changes in a bipartite bank network: a new perspective on the Japanese banking crisis of the 1990s (+ erratum)
- Network topology of the Argentine interbank money market
- On the transaction dynamics of the Ethereum-based cryptocurrency

**Representative medium-aligned:** Adaptive spectral community detection in temporal networks: a modularity optimization framework with memory and smoothing · Detecting periodic time scales of changes in temporal networks · Skeleton coupling: a novel interlayer mapping of community evolution in temporal networks · Null models for community detection in spatially embedded, temporal networks · Topological–temporal properties of evolving networks.

### 3.2 Centre of gravity — the thing you were worried about

JoCN's stated scope covers "Mathematical and numerical analysis of networks", "Structural analysis of networks", "**Social, socio-economic and political networks**", "Evolving networks", and — the catch-all that matters — "**Other nontrivial applications of networks which represent significant advances in the field**."

The journal is more mathematically inclined than ANS, and the operative word in its aims is "**significant contribution**." But the census is unambiguous: it publishes **purely empirical market-network case studies with no new mathematics** (the Indian, Brazilian and Argentine market papers), *and* it publishes methodological work on correlation-network construction and filtering (return correlation networks, testing randomness of correlation networks, Pearson correlations on complex networks, all-minimum-spanning-trees algorithms). Your paper is a methodological contribution plus an empirical demonstration. That is a better match to JoCN's taste than a pure case study would be.

**Your fear about JoCN is not supported by the data.** It is a good fit.

### 3.3 Fit score — **7.5 / 10**

| Sub-score | Score | Justification |
|---|---|---|
| Scope match | 8/10 | "Socio-economic networks" and "other nontrivial applications … which represent significant advances" both cover it. Slightly more theory-hungry than ANS, hence 8 not 9. |
| Methodological fit | 8/10 | The journal has published MST algorithms, correlation-network randomness tests and Pearson-correlation network work. Your toolkit is native here. |
| Novelty | 7/10 | Gap holds, but "The origin of return correlation networks" and "Testing the randomness of correlation networks from multivariate time series" raise the bar. Engage both explicitly or a reviewer will position your criterion as a variant. |
| Expected reviewer reception | 7/10 | Two single-anonymised reviewers, likely one applied-finance and one network-methods. The methods reviewer will want the criterion justified more formally than "it satisfies three desiderata." |
| Audience interest | 8/10 | Real, established finance-networks readership. Slightly narrower and more mathematical than ANS. |

**Verdict: submit-after-revisions** — specifically, sharpen the formal justification of the criterion (§8, items 1–3).

### 3.4 Difficulty & speed

| Metric | Value | Source |
|---|---|---|
| Impact Factor (2025) | **1.9** | OUP About page |
| 5-year IF (2025) | **2.4** *(higher than ANS)* | OUP About page |
| CiteScore (2025) | **2.8** | OUP About page |
| Category rank | **64/137**, Mathematics Interdisciplinary Applications | OUP About page |
| SNIP (2025) | 0.682 | OUP About page |
| Cited half-life | 6.1 years | OUP About page |
| Articles/year | ~52 (six issues/year) | Crossref + OUP |
| Acceptance rate | Not disclosed | — |
| Time to first decision | **Not disclosed** — estimate 2–4 months | Estimate, flagged as such |
| Time to publication after acceptance | Fast: "the journal publishes continuously by issue" | OUP author instructions |
| Peer review | Single anonymised, typically **two** reviewers | OUP author instructions |
| OA model | **Hybrid** — "the option of publishing under either a standard licence or an open access licence" | OUP author instructions |

**Prestige read:** JoCN edges ANS on 5-year IF (2.4 vs 2.2) and carries an OUP imprint plus a real Clarivate category rank. On the "decently prestigious" criterion, JoCN is at least ANS's equal and arguably better regarded in mathematical-sciences circles — which matters for a Loughborough/Imperial maths department.

**Practical friction:** JoCN wants LaTeX `article.cls` with text width 30 picas and page depth 46 picas, and abstract ≤300 words with up to six keywords. Your manuscript is RevTeX two-column. Budget half a day for reformatting. There is also a free Paperpal Preflight technical check for the journal — use it.

### 3.5 What a sharp JoCN reviewer will most probe

1. **"Is the MST max edge weight principled or merely convenient?"** Expect a demand for something closer to a proof or a stated optimality property — at minimum, an explicit statement that it is the *infimum* of thresholds yielding a connected graph, with that framed as a formal property rather than an observation.
2. **"How does this relate to significance-based and cross-validation-based filtering?"** The journal has published exactly that alternative. Address it head-on.

---

## 4. Network Science (Cambridge University Press, ISSN 2050-1242 / 2050-1250)

### 4.1 Alignment table

| Tier | Count | Share of 429 |
|---|---|---|
| **Heavily aligned** | **~3** | **~0.7%** |
| **Medium aligned** | ~32 | ~7.5% |
| Low aligned | remainder | — |

**Heavily aligned — the complete list. This is the whole set, from 13 years and 429 papers:**

- Has bitcoin been dethroned too quickly? The cryptocurrency return networks — *the only return-correlation-network paper in the journal's history*
- Reengineering of interbank networks
- Static and dynamic networks in interbank markets

**Methodologically adjacent but non-financial:** Generating weighted and thresholded gene coexpression networks using signed distance correlation — worth citing as evidence the *thresholding problem* is recognised here, but it is a gene-expression paper.

Note what is **absent**: not one paper on stock correlation networks, MST filtering, PMFG/TMFG, market crises via network structure, or econophysics. Two of the three "heavily aligned" papers are about interbank *balance-sheet* networks — a different object entirely (real counterparty edges, not inferred correlation edges).

**Representative medium-aligned (this is where the journal actually lives):** A theoretical and empirical comparison of the temporal exponential random graph model and the stochastic actor-oriented model · Random effects in dynamic network actor models · Choosing the number of groups in a latent stochastic blockmodel for dynamic networks · Simultaneous and temporal autoregressive network models · Accounting for edge uncertainty in stochastic actor-oriented models · Social cohesion emerging from a community-based physical activity program: A temporal network analysis · Social networks and labor market inequality between ethnicities and races.

### 4.2 Centre of gravity — why this is the wrong room

The journal describes itself as "focused on inspiring applications of network approaches, **rigorous theory building**, and innovative methods."

The census shows two dominant clusters: (a) **statistical models for network data** — ERGM, TERGM, SAOM, latent stochastic blockmodels, network autocorrelation models, dynamic network actor models; and (b) **social-science network applications** — sociology, political science, co-authorship, criminology, labour markets. Its temporal-networks work is overwhelmingly *inferential statistical modelling of tie formation*, not *structural analysis of inferred correlation graphs*.

Your paper has no statistical model, no likelihood, no inference on tie formation, and no theorem. It is a descriptive structural analysis of a filtered correlation graph. To this readership it will read as competent but methodologically thin — which is, uncomfortably, a close cousin of Physica A Reviewer #4's "some basic network metrics" complaint. **Sending it here risks a third rejection for the same underlying reason as the first two: right science, wrong room.**

At ~25 papers/year it is also the most selective of the three by volume, and its quarterly schedule means a slower path from acceptance to issue.

### 4.3 Fit score — **5.0 / 10**

| Sub-score | Score | Justification |
|---|---|---|
| Scope match | 5/10 | "Inspiring applications of network approaches" nominally admits it; "rigorous theory building" and the actual catalogue push against it. |
| Methodological fit | 6/10 | Louvain/modularity/centrality are recognised, but the house style is statistical network modelling, which your paper does not do. |
| Novelty | 7/10 | The gap is the *widest* of the three — but a wide gap in a journal whose readers don't work on the problem is a liability, not an asset. Reviewers read unfamiliarity as "why here?" |
| Expected reviewer reception | 4/10 | Likely reviewers are sociologists or statisticians of networks. High risk of "interesting but not a contribution to network science as this journal understands it." |
| Audience interest | 4/10 | Three finance papers in 429. There is no waiting readership. |

**Verdict: reconsider venue.** Free publication does not compensate for a fit this weak, and a third rejection costs you 4–6 months.

### 4.4 Difficulty & speed

| Metric | Value | Confidence |
|---|---|---|
| Impact Factor | **Not published on the CUP journal page.** A partial automated check returned 1.6 (2025 JCR) — **unverified, confirm before relying on it** | Low |
| CiteScore / SJR | Not published on the journal page | — |
| Articles/year | ~25 (88 records since Jan 2023) | High (Crossref) |
| Acceptance rate | Not disclosed | — |
| Time to first decision | Not disclosed — estimate 3–5 months for a small quarterly | Estimate |
| OA model | Hybrid / gold OA option — **confirm whether it sits on CUP's "Journals containing open access" (hybrid) list or the "Research Open" (fully OA) list**, since this determines read-and-publish eligibility | Medium |

**Caveat:** CUP does not publish citation metrics or turnaround times on the Network Science journal page, so this row is the least well-evidenced of the three. That itself is worth noting — the two journals that *do* publish their speed figures are the two I'm recommending.

---

## 5. Novelty & gap analysis (applies to all three)

**The claim:** no paper in any of the three journals — and, as far as the literature you cite goes, no paper anywhere — selects the threshold for a correlation-based threshold network **per time window, automatically, as the maximum edge weight of that window's MST**, thereby guaranteeing a connected graph at the sparsest possible threshold, and applies it across ~500 rolling windows on 2,456 assets.

**Does the gap hold? Yes — but narrowly, and you are currently under-selling it.**

The three closest competitors anywhere:

1. **Xu et al.** — choose a *single global* threshold applied across the whole period, maximising the correlation between changes in the threshold network and changes in the weighted network. Your differentiator: per-window adaptation. **You state this. Good.**
2. **Ku et al.** — union of MST edges with all edges below a prescribed distance threshold. Guarantees connectivity, but still leaves the threshold free. Your differentiator: you *derive* the threshold instead of prescribing it, which is what makes it usable across hundreds of windows. **You state this. Good.**
3. **Nobi et al.** — threshold from the mean and standard deviation of the correlation coefficients. Your differentiator: distribution-free, no tuning constant.

**Where you under-sell, and it is costing you:**

- The abstract calls it "a criterion proposed for selecting a suitable threshold." That is the language of a minor methodological aside. It is your primary contribution and it is **domain-agnostic** — the paper says so ("does not depend on the nature of the data that is analyzed and can therefore be applied across diverse fields of study") and then buries it in the middle of the introduction. In an *applied network science* journal, "a threshold-selection rule for any temporal correlation network, demonstrated on the largest single-market stock network yet analysed" is a much stronger claim than "a Covid-19 study."
- You never state the property that makes the criterion clean: **the MST's maximum edge weight is precisely the infimum of thresholds at which the threshold graph is connected.** That is a one-line, exact statement. Say it as a formal property. It converts "heuristic that works" into "the unique minimal connected threshold," which is what a JoCN methods reviewer is looking for.
- The **out-of-sample validation** (threshold criterion re-evaluated on post-Oct-2021 data, "results are similar to those shown") is buried in a single sentence at the end of §II. That sentence answers Physica A Reviewer #4's most substantive methodological objection. Promote it.
- Threshold stability — "always close to 0.98, with a standard deviation of approximately 0.03" — is a genuinely strong empirical result and appears as an aside. It is evidence the criterion is well-behaved, which is exactly what a reviewer doubting its principledness needs.

**Threats you must cite and differentiate from (currently, as far as I can tell, uncited):**

| Paper | Journal | Why it threatens you |
|---|---|---|
| Cross-validation of correlation networks using modular structure | Applied Network Science | A competing principled method for validating correlation-network filtering, using modular structure — the same quantity you use to justify your threshold |
| Testing the randomness of correlation networks from multivariate time series | J. Complex Networks | The significance-filtering alternative: keep statistically non-random edges. A reviewer will ask why your criterion is preferable |
| The origin of return correlation networks | J. Complex Networks | Directly on the object you study; establishes the journal's prior on return correlation networks |
| Threshold sensitivity of the production network topology | Applied Network Science | Establishes that ANS already cares about threshold choice — helps you, but you must not appear unaware of it |

Adding these four citations does three things at once: closes the novelty gap credibly, signals venue fit, and pre-empts the "insufficient novelty" line that got you desk-rejected at CSF.

---

## 6. Mining the rejection history

**Physica A (PHYSA-24982R1, reject; editor Michael Small).** Two reviewers, one of whom — Reviewer #6 — explicitly wrote that the work "**may be publishable** in this journal." That is not a hostile review. Every technical point raised has since been addressed in the current manuscript. These are now **strengths to surface prominently**, not open weaknesses:

| Original objection | Current status | Where to surface it |
|---|---|---|
| Threshold percentile sensitivity (95th/97th/99th) | Addressed — Figs 2–4 show components, edge share and modularity as continuous functions of threshold | Already in §II.C.2; reference from the abstract |
| Scale-free claim needs statistical validation | Addressed / offending claim removed | Cover letter |
| Optimal threshold should be identified outside the analysis period | Addressed — criterion re-evaluated on post-Oct-2021 data | §II, promote to abstract |
| Window-asymmetry justification (6-month pre vs longer post) | Addressed — §II.A now explains the deliberate choice of a stable 6-month pre-onset period plus a recovery period | §II.A |
| Monthly averaging may smooth the analysis | Addressed — analysis now runs on rolling 21-day windows starting on *every* trading day | §II.B — this is a real strength; say so |
| Figure formats, missing lead-in text, PMFG vs TMFG | Addressed / material removed | Cover letter |

Reviewer #4's "limited to the North-American market with some basic network metrics" is a **scope-and-taste objection appropriate to a statistical-mechanics journal**, not a technical flaw. Note, though, that it is the *same* objection Network Science's readership would raise — which is the core of my recommendation against Network Science.

**Chaos, Solitons & Fractals (CHAOS-D-26-00118, desk reject; editor Tiziana Di Matteo).** Internally contradictory: the scope field says the subject "does not fall within the scope of the journal" while the comments to authors say it "falls within the aim and scope" but is declined for "lack of sufficient novelty… We receive a much larger number of papers than we are able to accept." That is **boilerplate on a volume-driven desk reject with no technical review of your network analysis.** Do not treat it as a novelty verdict. Do, however, treat it as a warning that the novelty claim needs to be unmissable in the first two sentences of the abstract — a busy editor triaging on volume never got past your framing.

**The pattern is the argument.** Two rejections, both from nonlinear-physics / statistical-mechanics venues, neither on the substance of the network analysis. This is a textbook applied-network-science paper that has twice been sent to physics journals. Both ANS and JoCN are the correct class of venue; the rejection history is evidence *for* them, not against you. State this plainly in your cover letter — editors respect a candid, well-reasoned venue-choice narrative.

---

## 7. Head-to-head comparison

| | **Applied Network Science** | **Journal of Complex Networks** | **Network Science** |
|---|---|---|---|
| **Fit score** | **8.5/10** | **7.5/10** | **5.0/10** |
| Publisher | Springer Nature | Oxford University Press | Cambridge University Press |
| Impact Factor (2025) | 1.9 | 1.9 | Not published (unverified 1.6) |
| 5-year IF | 2.2 | **2.4** | Not published |
| CiteScore | Not published | **2.8** | Not published |
| Category rank | — | 64/137 Math Interdisc. Appl. | — |
| Heavily aligned papers | ~16 / 802 (2.0%) | ~13 / 638 (2.0%) | **~3 / 429 (0.7%)** |
| Closest existing paper | Cross-validation of correlation networks | **The origin of return correlation networks** | Cryptocurrency return networks |
| Articles/year | ~80 | ~52 | ~25 |
| **Median time to first decision** | **14 days (published)** ✅ | Not disclosed (est. 2–4 months) | Not disclosed (est. 3–5 months) |
| Time to publication after acceptance | Immediate (OA, continuous) | Fast (continuous by issue) | Slower (quarterly) |
| Acceptance difficulty | **Most forgiving** | Moderate | **Hardest for this paper** |
| Reviewers | Not stated | 2, single anonymised | Not stated |
| OA model | **Fully OA** | **Hybrid** | Hybrid / gold option |
| APC | **£1,240 / $1,790 / €1,490** + VAT | Free under R&P (verify) | Free under R&P (verify) |
| Prestige for a maths dept. | Good | **Best** (OUP + Clarivate rank) | Good name, wrong field |
| Formatting effort | Low | Moderate (`article.cls`, 30×46 picas) | Moderate |
| **Recommendation** | **Submit if APC funded** | **Submit — default choice** | **Do not submit** |

### The trade-off in one paragraph

ANS wins on raw fit and on speed-to-first-decision by a wide, *documented* margin. JoCN matches it on prestige (better on 5-year IF and CiteScore, with a real Clarivate category rank), is only one point behind on fit, costs nothing, and has the single closest-matched existing readership for a return-correlation-network paper. Network Science loses on every axis that matters here except cost, and cost is the axis where it ties with JoCN — so it is strictly dominated. **Given that your priorities are speed, decent prestige, reasonable acceptance odds and affordability, JoCN is the choice that satisfies all four simultaneously; ANS satisfies three brilliantly and one only if someone else pays.**

---

## 8. Open access and funding

**Confirmed facts:**

| Journal | OA model | APC (list) | Source |
|---|---|---|---|
| Applied Network Science | **Fully open access** (SpringerOpen) — an APC applies to every accepted article; there is no subscription route | **£1,240 / $1,790 / €1,490** + VAT | Springer "How to publish with us" |
| Journal of Complex Networks | **Hybrid** — standard licence or optional OA licence | £0 via standard licence; OA charge only if you choose OA | OUP author instructions |
| Network Science | Hybrid / gold option — confirm which CUP list it sits on | £0 via standard licence | CUP journal page |

**The good news on ANS:** £1,240 is at the low end for a fully-OA title — well under half of *Scientific Reports* or *EPJ Data Science*. If there is any discretionary research account, this is a small ask.

**The trap you need to check, and I could not resolve it for you.** UK Jisc read-and-publish deals reliably cover **hybrid** journals (which is why JoCN and Network Science are "free via the uni"). They frequently **exclude, or only discount, fully open-access titles** — and Springer Nature has historically run separate arrangements for hybrid Springer journals versus its fully-OA SpringerOpen/BMC portfolio. Applied Network Science is a fully-OA SpringerOpen title, so **whether it is £0 or £1,240 for you is exactly the question the general deal does not settle.**

I could not verify this. Springer's per-journal eligibility checker (`link.springer.com/journal/41109/funding-eligibility`) requires JavaScript form interaction, and the Imperial, Loughborough and Jisc agreement pages all returned client-rendered shells to my fetcher. **Do not act on an assumption here.**

**Three things to do before you submit anywhere:**

1. **Run Springer's checker yourself** at `link.springer.com/journal/41109/funding-eligibility`, selecting *Imperial College London*, then again selecting *Loughborough University*. It answers the £0-vs-£1,240 question definitively in about thirty seconds. Also check Imperial's SciFree tool at `search.scifree.se/imperial`.
2. **Email the Imperial open-access team** with the journal name and ISSN 2364-8228, asking specifically whether *fully open-access SpringerOpen titles* are covered under Imperial's Springer Nature agreement, or only discounted. Ask the same of Loughborough's library. Ask about institutional OA funds for DOAJ-listed journals as a fallback — ANS is DOAJ-listed, which usually satisfies those funds' eligibility rules.
3. **Settle the corresponding-author question before submission, not after.** OUP states explicitly that "changing the corresponding author in order to access Read and Publish funding is not permissible." You are at Imperial; the manuscript lists Loughborough. Decide now which institution's agreement you are claiming, list that affiliation, and be the corresponding author from the first submission. Retrofitting this after acceptance will be refused. Listing both affiliations for yourself is normal and honest, but the corresponding-author institution is what the deal keys on.

**Decision rule:** if the checker says Imperial or Loughborough covers ANS → submit to **ANS**, today's best combination of fit and speed. If it says not covered and £1,240 is not readily available → submit to **JoCN** without hesitation. You are giving up roughly one point of fit and gaining a slightly better 5-year IF, for free.

---

## 9. Alternatives — is anything better than these three?

**Direct answer: no.** Nothing I examined clearly beats ANS or JoCN on your combined criteria of speed, prestige, acceptance odds and cost. Two are worth holding in reserve; several commonly-suggested options are worse than they look.

**Confidence note:** the metrics in this section are from my working knowledge and were **not verified against publisher pages in this run** (the three target journals were). Treat them as directional and verify before acting.

### Hold in reserve

| Venue | Publisher / model | Why it's worth holding |
|---|---|---|
| **Journal of Physics: Complexity** | IOP, fully OA | Genuinely good topical fit — publishes network structure and complex-systems applications including financial networks; IOP has UK transformative arrangements worth checking, which could make it free. Younger and lower-profile than JoCN. **Best reserve option.** |
| **Journal of Economic Interaction and Coordination** | Springer, **hybrid** | Explicitly econophysics-and-agent-based friendly; hybrid, so very likely free to you under the Springer deal. Small and slower, lower IF, narrower readership. **Best free-and-friendly backup after JoCN.** |
| **EPJ Data Science** | Springer, fully OA | Higher prestige than all three targets and a real appetite for temporal/financial network analysis. But more selective, a higher APC, and it wants a data-science contribution framing. Only if you want to reach up and can wait. |
| **Quantitative Finance** | Taylor & Francis, hybrid | Prestigious in finance and covered by the Jisc T&F deal. Risky: reviewers are financial economists who will ask what the *economic* contribution is, and "market structure changed during Covid" may not satisfy them. Consider only after a JoCN acceptance-shaped rewrite. |

### Approach with caution

- **Scientific Reports** — accepts technically sound work with light novelty demands and would very likely take this. But the APC (~£1,690, higher than ANS) buys you *less* topical readership than ANS, and a network-methods paper there is easily lost. Poor value given ANS is cheaper and better matched.
- **Entropy (MDPI)** — fast, publishes econophysics, and would probably accept. But the APC is high (~CHF 2,600), it is not covered by UK deals, and MDPI titles attract quality scepticism in mathematics and physics departments. Given that your problem is *perceived novelty*, publishing somewhere with a reputation discount actively works against you.
- **PLOS ONE** — will publish sound science, but the venue signals "couldn't place it elsewhere" to a maths readership, and the APC is not trivial.
- **Frontiers in Physics (Social Physics)** — fast and topically plausible, but APC-funded and carries similar reputational caveats to MDPI in this field.
- **Finance Research Letters / International Review of Financial Analysis** — high IFs and fast, but they want short papers with an identified *financial-economics* contribution and an empirical hypothesis. Your paper is a methods paper. High desk-reject risk on framing.

### Actively advise against

- **Physica A** — already rejected. Do not resubmit; the same editorial office and likely the same reviewer pool.
- **Chaos, Solitons & Fractals** — already desk-rejected on scope and volume. Do not resubmit.
- **Any physics-first venue at all** (EPJ B, Physica Scripta, J. Stat. Mech.). They are hybrid and therefore free to you, which is tempting. But you have now been rejected twice by exactly this class of journal for exactly the reason that they want physical insight or new nonlinear phenomena and your paper offers a practical method. **Going back to the well a third time is the single most likely way to lose another six months.**
- **Complexity (Wiley/Hindawi)** — the Hindawi legacy carries serious paper-mill and mass-retraction associations. Avoid.
- **Journal of Network Theory in Finance** — check whether it is still actively publishing before spending any time on it; low volume and limited visibility.

**If all three current candidates failed**, submit in this order: **(1) Journal of Physics: Complexity**, **(2) Journal of Economic Interaction and Coordination**, **(3) EPJ Data Science**.

---

## 10. Framing, title and cover-letter advice

### Ranked candidate titles

The current title — "The Covid-19 Impact on Temporal Threshold Networks in the US Stock Market" — leads with the *application* and puts the contribution nowhere. That framing is a plausible part of why a volume-triaging editor read it as a Covid case study and reached for the novelty boilerplate. **Lead with the method.**

1. **"A minimum-spanning-tree criterion for thresholding temporal correlation networks, with application to the Covid-19 US stock market"** — best for both ANS and JoCN. Method first, domain-agnostic, application as demonstration. Contains every keyword a matched reviewer searches on.
2. **"Automatable threshold selection for temporal correlation networks: the Covid-19 collapse of US stock market diversification"** — slightly punchier; "automatable" is your real selling point and "collapse of diversification" is the memorable finding.
3. **"Thresholding temporal financial correlation networks via the minimum spanning tree: Covid-19 and the structure of the US market"** — good for JoCN specifically; "financial" signals the finance stream, MST signals the methods stream.
4. **"Temporal threshold networks reveal the Covid-19 collapse and recovery of US stock market diversification"** — only if you decide to lead with the application. Not recommended for these venues.

Avoid: any title beginning "The Covid-19 Impact on…". It reads as a case study and invites the novelty objection you have already received twice.

### Abstract surgery (the highest-leverage change in this whole report)

Restructure to: **(1)** threshold choice is the central unsolved practical problem for temporal correlation networks — one sentence; **(2)** we propose the MST's maximum edge weight, which is exactly the smallest threshold giving a connected network, requires no tuning, is automatable, and is **domain-independent** — two sentences; **(3)** we validate it on threshold sensitivity and out-of-sample data, finding it stable at 0.98 ± 0.03 — one sentence; **(4)** applied to 2,456 NASDAQ stocks across the Covid-19 crash it reveals a temporary collapse of market diversification and recovery by late 2020 — two sentences; **(5)** implications for systemic-risk monitoring — one sentence.

Your current abstract puts the criterion in a subordinate clause of the fifth sentence. Move it to the second.

### Reviewer search terms to include in the keyword list

`threshold networks` · `minimum spanning tree` · `temporal networks` · `correlation networks` · `community detection` · `modularity` · `systemic risk` · `econophysics` · `market structure` · `Covid-19`

For JoCN you get six keywords — use: *temporal networks, threshold networks, minimum spanning tree, correlation networks, community detection, systemic risk*. Note that "econophysics" is a keyword that helps you at ANS and hurts you at Network Science; drop it if you ever do submit to CUP.

### Framings to avoid

- Don't foreground "nonlinear dynamics", "phase transition", or "critical phenomena" language. It reads as physics-journal framing and you are deliberately leaving that room.
- Don't describe the paper as revealing "hidden impacts" of Covid-19 (current abstract). It sounds like a finding-hunting case study. It reveals the *collapse of diversification*, which is specific and defensible.
- Don't apologise for the single-market scope. Reframe it as a strength: the *entire* NASDAQ, 2,456 stocks, every trading day over two years — this is one of the largest single-market temporal correlation-network analyses published, and it is what makes the automatability claim meaningful. Then note generalisation to other markets as future work, in one sentence, pre-empting Physica A Reviewer #6's point 6.

### Papers to cite to signal fit

**For ANS:** Cross-validation of correlation networks using modular structure · Threshold sensitivity of the production network topology · Network-based diversification of stock and cryptocurrency portfolios · Characterizing financial markets from the event driven perspective · Correlation networks of air particulate matter (PM₂.₅) — this last one is strategically excellent, because it demonstrates to an ANS editor that a domain-agnostic threshold criterion serves readers well outside finance.

**For JoCN:** The origin of return correlation networks · Testing the randomness of correlation networks from multivariate time series · Pearson correlations on complex networks · Analyzing communicability and connectivity in the Indian stock market during crises · Adaptive spectral community detection in temporal networks.

### Cover letter — three things to say

1. **Name the contribution in the first sentence** as a general threshold-selection criterion for temporal correlation networks, not a Covid-19 study.
2. **Own the submission history briefly and confidently.** One or two sentences: the paper was previously reviewed at Physica A, where all technical points — threshold-percentile sensitivity, statistical validation, out-of-sample threshold selection, window-asymmetry justification — have been addressed in this version; the paper was subsequently declined on scope at a nonlinear-dynamics venue; you are now submitting to an applied-network venue because the contribution is methodological and applied rather than a contribution to nonlinear physics. Editors read this as good judgement, not as damaged goods.
3. **Suggest reviewers** from the aligned-paper lists above. Authors of the return-correlation-network and threshold-sensitivity papers are ideal: they are competent to assess the criterion and predisposed to think the problem matters.

---

## 11. Revision checklist, in priority order

**Must do before submitting anywhere** *(roughly 2–3 days)*

1. **Rewrite the abstract** to lead with the criterion (§10). Highest leverage single change in this report.
2. **Change the title** to option 1 or 2.
3. **State the formal property explicitly:** the MST's maximum edge weight is the infimum of thresholds for which the threshold graph is connected. One sentence, stated as a property. This is what converts a heuristic into a criterion in a methods reviewer's eyes.
4. **Promote the out-of-sample validation** (post-Oct-2021 re-evaluation) from a closing aside in §II to the abstract and to a named paragraph. It answers the strongest prior objection you have received.
5. **Promote the threshold-stability result** (0.98 ± 0.03 across all windows) to a headline finding.
6. **Add the four threat citations** (§5) and differentiate from each in one or two sentences.

**Should do — materially improves acceptance odds** *(roughly 3–5 days)*

7. **Add one benchmark figure** comparing your criterion against Xu et al.'s global threshold and Ku et al.'s MST-union on the same data — e.g. modularity and component count over time under each. This closes the "is it actually better?" question that both an ANS and a JoCN reviewer will ask, and it is the largest remaining gap in the paper.
8. **Add a short "generality" paragraph** applying the criterion to one non-financial correlation time series, or at minimum spelling out the recipe domain-agnostically. Turns a finance paper into a methods paper with a finance demonstration — which is what both target journals reward.
9. **Add one sentence on international generalisation** as future work (pre-empts Physica A Reviewer #6 point 6).
10. **Soften remaining physics framing** in the introduction and conclusion.

**Venue-specific**

11. *If JoCN:* reformat from RevTeX to `article.cls`, text width 30 picas, page depth 46 picas; abstract ≤300 words; ≤6 keywords; run the free Paperpal Preflight check; add alt text for every figure (required at submission); prepare the Funding section in OUP's exact format.
12. *If ANS:* Springer submission format; confirm the funding position first (§8); submit to the general track, not a collection.
13. **Either way:** resolve the corresponding-author/affiliation question before you submit (§8, item 3).

---

## 12. Caveats

- **Tiering is title-based.** Abstracts were not read, so each tier count carries roughly ±3–4 papers of uncertainty. Direction and rough magnitude are reliable; exact counts are not.
- **Crossref totals include non-article records** (editorials, corrections, front matter), so articles/year figures are slight over-counts. All three journals are counted the same way, so the comparison holds.
- **Network Science's citation metrics and turnaround times are not published** on its CUP journal page. The IF of 1.6 appearing in §4.4 came from an incomplete automated check and is explicitly **unverified**. Its OA classification (hybrid vs CUP "Research Open") also needs confirming.
- **The funding question is unresolved** and is the one input that changes the recommendation. Springer's eligibility checker and the Imperial, Loughborough and Jisc agreement pages are all JavaScript-rendered and returned no content to my fetcher; browser automation was unavailable in this session. §8 tells you exactly which three checks to run.
- **§9 alternatives were not verified** against publisher pages in this run. Impact factors, APCs and turnaround times there are directional only.
- Confirmed and dated in this run: ANS metrics and APC (Springer journal and "How to publish with us" pages), JoCN metrics and hybrid OA status and peer-review process (OUP About and General Instructions pages), all three Crossref censuses, and the manuscript content (read directly from the PDF).

**Sources:** Crossref REST API (`api.crossref.org`, queried 31 July 2026, ISSNs 2364-8228 / 2051-1329 / 2050-1250) · [Applied Network Science — journal home](https://link.springer.com/journal/41109) · [Applied Network Science — How to publish with us](https://link.springer.com/journal/41109/how-to-publish-with-us) · [Applied Network Science — open access funding](https://link.springer.com/journal/41109/funding-eligibility) · [Journal of Complex Networks — About](https://academic.oup.com/comnet/pages/About) · [Journal of Complex Networks — Instructions to Authors](https://academic.oup.com/comnet/pages/General_Instructions) · [Network Science — CUP journal home](https://www.cambridge.org/core/journals/network-science) · manuscript PDF as supplied.
