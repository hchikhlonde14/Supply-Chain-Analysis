\# Supply Chain Delivery Performance Analysis



End-to-end order fulfillment analysis and predictive insights for a global e-commerce operation covering \*\*172,765 orders\*\* (January 2015 – January 2018).



\---



\## 📊 Key Metrics



| Metric | Value |

|---|---|

| Total Orders Analyzed | 172,765 |

| Late Delivery Rate | \*\*54.71%\*\* |

| On-Time Delivery Rate | 45.29% |

| Total Profit (profitable orders) | $7.5M |

| Profit at Risk (delayed orders) | $2.1M |

| Average Order Profit | $22.03 |

| 90th Percentile Delay | 3 days |

| Predictive Model Accuracy (Random Forest) | 74% |



\---



\## 🔍 Key Findings



\### Profitability

\- \*\*80.7%\*\* of orders are profitable, \*\*18.7%\*\* are loss-making, and \*\*0.6%\*\* break even.

\- Mean profit per order is stable at \~$20–$23 regardless of delay length — the financial problem is driven by \*\*volume\*\*, not individual order economics.

\- The largest delay cohort is orders arriving exactly \*\*1 day late\*\* (31.0% of all orders).



\### Bottlenecks by Shipping Mode

Shipping mode is the single most impactful variable:



| Mode | Delay Rate |

|---|---|

| First Class | \*\*100%\*\* |

| Second Class | 79.8% |

| Standard Class | 39.8% |

| Same Day | 0% |



\### Regional \& Segment Performance

\- All regions cluster tightly between \*\*55–59%\*\* delay rate, confirming a \*\*company-wide systemic issue\*\* rather than a localized failure.

\- All customer segments (Consumer, Corporate, Home Office) experience the same delay rates (54.5–55.4%) — no segment receives preferential service.

\- Health \& Beauty (56.9%) and Pet Shop (56.6%) are the highest-delay departments.



\### Time-Based Patterns

\- \*\*Peak delay months:\*\* August \& September (55.4%), December (55.2%) — driven by mid-year promotions and holiday surge.

\- \*\*Intra-day peak:\*\* Hour 21 (57.1%), likely tied to processing cutoff windows.

\- Day-of-week variance is negligible (<1 percentage point).



\### Root Cause Analysis (Central Africa — highest-delay region at 58.7%)

Top drivers of late delivery:

1\. Shipping Mode: First Class — \*\*100%\*\*

2\. Shipping Mode: Second Class — \*\*82.8%\*\*

3\. Order Status: PAYMENT\_REVIEW — \*\*80.0%\*\*

4\. Order Status: PENDING — \*\*69.1%\*\*

5\. Department: Outdoors — \*\*61.3%\*\*



\---



\## 🤖 Predictive Model



A \*\*Random Forest classifier\*\* was trained to flag at-risk orders before shipment.



| Metric | On-Time (Class 0) | Late (Class 1) | Overall |

|---|---|---|---|

| Precision | 0.68 | \*\*0.78\*\* | 0.74 |

| Recall | 0.72 | 0.75 | 0.74 |

| F1-Score | 0.70 | 0.77 | 0.74 |



\*\*SMOTE oversampling\*\* was applied to address class imbalance in training data. The model is considered ready for production piloting as an order-level alert system.



\---



\## ✅ Strategic Recommendations



| Priority | Action |

|---|---|

| 🔴 Critical | Audit First Class \& Second Class carrier SLAs immediately; consider suspending First Class |

| 🟠 High | Deploy the predictive alert system into the order management platform |

| 🟠 High | Automate escalation for payment reviews stalled beyond 2 hours |

| 🟡 Medium | Build seasonal surge capacity plans for August, October, and December |

| 🟡 Medium | Default eligible orders to Standard Class shipping |

| 🟡 Medium | Warehouse audit for Outdoors \& Golf departments in Central Africa |

| 🟢 Low | Review pricing/discounts to reduce the 18.7% loss-making order share |

| 🟢 Low | Retrain the predictive model quarterly; target >80% recall within 6 months |



\---



\## 🎯 Targets



| Area | Current | Target |

|---|---|---|

| Late Delivery Rate | 54.71% | < 30% within 12 months |

| First Class On-Time Rate | 0% | > 80% |

| Second Class On-Time Rate | 20.2% | > 60% |

| Predictive Model Accuracy | 74% | > 82% |

| Loss-Making Orders | 18.7% | < 12% |

| Profit at Risk | $2.1M | Reduce by 40% |



\---



\## 📁 Report Structure



```

1\. Executive Summary

2\. Business Context \& Objectives

3\. Key Performance Indicators (KPIs)

4\. Profitability Analysis

&#x20;  4.1 Profitability Distribution

&#x20;  4.2 Delay Distribution \& Profit vs. Delay Days

5\. Bottleneck Detection

6\. Root Cause Analysis

7\. Time-Based Delay Patterns

8\. Machine Learning Model Results

9\. Strategic Recommendations

10\. Conclusion

```



