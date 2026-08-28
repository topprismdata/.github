# TopPrism public evidence cases

> **Language / 语言:** English primary · 中文摘要 included below。

This page collects publicly stated evidence from selected TopPrism
repositories. The figures are **repository-reported study or validation
results**, not a universal performance guarantee or a claim that all projects
are one deployed product.

## Case 1 — Spatial data trust and readiness

Repository: [`spatial-decision-intelligence`](https://github.com/topprismdata/spatial-decision-intelligence)

The repository reports an end-to-end validation across **9,039 operational
enterprise geofences** in Beijing and Shijiazhuang:

- 8,332 WGS-84 point / GCJ-02 polygon offsets corrected;
- 505 missing points rebuilt from centroids;
- 539 self-intersecting polygons healed;
- 838 degenerate industrial slivers identified;
- 4,931 soft candidate pairs re-scored with a BGE cross-encoder;
- zero automatic merges executed; human governance remained the red line.

**中文摘要：**该项目把空间数据质量、边界生成和决策就绪度作为 Business World Model 的基础，
验证重点是诊断与人工复核，不是自动宣称下游片区一定最优。

**Boundary:** the evidence supports diagnosis and readiness gating. It does
not prove that downstream territory allocations are automatically optimal, and
it does not replace procurement or human review.

## Case 2 — Recurring field-visit planning

Repository: [`visit-scheduling-optimizer`](https://github.com/topprismdata/visit-scheduling-optimizer)

The repository reports an anonymized industry study covering **7
representatives and 235 customers** over a 20-day horizon:

| Metric | Business actual | Framework | Reported change |
|---|---:|---:|---:|
| Active working days | 139 | 117 | -16% |
| In-day work hours | 768 h | 569 h | -26% |
| OSRM route distance | 10,056 km | 6,345 km | -37% |
| Frequency compliance | 92–100% | 100% | hard constraint satisfied |
| Daily work-hour-cap violations | 12% of days | 0% | hard constraint satisfied |

**中文摘要：**该项目把拜访频次、间隔、工时、路线和工作日约束显式建模，输出可复核的周期性拜访计划。

**Boundary:** these are study results, not a universal guarantee. Outcomes
depend on geography, frequency policy, depot location, workload rules and
travel-time calibration.

## Case 3 — Deterministic market geometry

Repository: [`market-partition`](https://github.com/topprismdata/market-partition)

The repository reports five Beijing validation cases using programmatic
landmark checks plus multimodal visual inspection:

| Case | Programmatic landmark result | Visual review |
|---|---:|---|
| Second Ring | 10/11 (91%) | ring visually closed |
| Third Ring | 10/11 (91%) | ring visually closed |
| Fourth Ring | 7/10 (70%) | ring visually closed |
| Fifth Ring | 9/10 (90%) | large ring visually complete |
| Chang'an Avenue | 5/5 (100%) | extended line spans region |

**中文摘要：**该项目让业务语言解释、确定性 GIS 几何和视觉复核形成闭环；不把语言模型当作几何计算器。

**Boundary:** imperfect landmark scores remain visible. Ambiguous labels and
geographic edge cases still require review; this is validation evidence, not a
claim of universal market-boundary accuracy.

## How to interpret these cases

Across the cases, TopPrism separates:

1. observed facts and measured outputs;
2. recommendations for human review;
3. approved decisions and downstream execution.

Use each repository README for method details, environments and the complete
non-goal statements. Use [`PORTFOLIO.yaml`](PORTFOLIO.yaml) for repository
roles and declared relationships.

Updated: 2026-08-28
