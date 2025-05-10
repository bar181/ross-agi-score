# Ross AGI Score (RAS)

**A Multidimensional Evaluation Framework for Artificial General Intelligence**
Draft Version v1.0   

Author: [Bradley Ross](mailto:brad.ross@quantinc.com) 
[`Contact`](https://www.linkedin.com/in/bradaross/) 
Lead AI/AGI Systems Architect & Developer  
Director, Agentics Foundation  
Harvard University, ALM Digital Media Design Candidate  

---

## ✨ Abstract

Artificial general intelligence (AGI) research lacks a unified, practical yard-stick that captures breadth, depth, and developmental progression in one view. The **Ross AGI Score (RAS)** fills that gap by combining (i) a **15-level AGI Capability Level (ACL) scale** —from minimal narrow automation (ACL 1) to theoretical maximal super-intelligence (ACL 15)—with (ii) a **multidimensional profile** covering core cognitive domains such as reasoning, learning, creativity, social understanding, and meta-cognition. Each level is anchored to empirically observable, behavior-based descriptors and calibrated against human benchmarks, with **ACL 10 defined as baseline human-level general intelligence**.

RAS outputs a single-page scorecard: individual ACL ratings per dimension plus an overall level derived from **minimum profile requirements** that prevent “savant” systems from being mis-classified as generally intelligent. Four milestone stages emerge naturally—*Narrow AI*, *Emergent AGI*, *Full AGI* (human-parity), and *Super-AGI*—enabling clear policy triggers and research goals.

We motivate RAS by surveying limitations of the Turing Test, single-task leaderboards, and existing psychometric approaches, then formalize every ACL band with qualitative anchors. A roadmap details creation of task batteries, human calibration studies, an open-source evaluation toolkit, and integration with governance frameworks. By delivering a transparent, human-referenced, profile-based metric, RAS provides researchers, developers, and policymakers a common language for tracking progress, diagnosing capability gaps, and managing risk as AI systems climb from narrow tools toward transformative super-intelligence.

Version 1.0 is released for public review and will form the basis of an upcoming arXiv submission; community feedback is encouraged.

---

## 📄 Overview

The **Ross AGI Score (RAS)** is a structured framework for evaluating AI systems on the path to Artificial General Intelligence. It introduces a 15-level **AGI Capability Level (ACL)** scale, spanning from narrow AI to extreme superintelligence. Each AI system is scored across multiple cognitive dimensions to form a capability **profile**, with **human-level general intelligence anchored at ACL 10**.

Key features:
- ✅ **15 ACL levels** with detailed behavioral descriptors  
- ✅ **Profile-based scoring** across multiple cognitive domains  
- ✅ **Human-calibrated milestones** (e.g. ACL 10 = human-level AGI)  
- ✅ **Minimum profile thresholds** for stage classification  
- ✅ **Scorecard format** for structured, transparent evaluations  

---

## 📘 Paper

The complete framework is documented in [`ross_agi_score.md`](ross_agi_score.md), covering:

- 15 AGI Capability Levels (ACL 1–15)  
- Cognitive dimension definitions and behavioral anchors  
- Stage classifications: Narrow AI, Emergent AGI, Full AGI, Super-AGI  
- Minimum profile requirements to classify AGI stages  
- Operationalization roadmap (evaluation suite, scoring, governance)  

Archived drafts are available in the `/archive/` folder for reference.

---

## 📊 RAS Scorecard

A conceptual 1-page scorecard format for practical evaluations is provided in [`scorecard_template.md`](scorecard_template.md). It includes:

- Cognitive dimension names and symbols  
- ACL rating columns (1–15 +)  
- Phase indicator (Rapid / Deep Dive)  
- Key evidence / justification fields  
- Final stage classification (e.g. Emergent AGI)  

---

## 🛠 Versioning

This repository includes:

- ✅ The most current **stable version** of the RAS paper (v1.0)  
- 🗂 Archived draft versions in `/archive/`  
- 🧪 Experimental tools and templates for future integration (planned)  

Future updates will use GitHub releases and include version tags (e.g. `v1.1`, `v2.0`).

---

## 🔍 License

All contents in this repository—including the paper, scoring templates, and descriptors—are licensed under the [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).

> ✅ Commercial use permitted  
> ✅ Modifications permitted  
> ❗ Attribution to the original author (Bradley Ross) required  

See [`LICENSE.md`](LICENSE.md) for full license terms.

---

## 💬 Citation

If referencing this work, please cite:

> Ross, Bradley. *The Ross AGI Score (RAS): A Multidimensional Evaluation Framework for Artificial General Intelligence*. 2025. Version 1.0. Available at: <https://github.com/bar181/ross-agi-score>

**BibTeX:**
```bibtex
@misc{ross2025ras,
  author       = {Bradley Ross},
  title        = {The Ross AGI Score (RAS): A Multidimensional Evaluation Framework for Artificial General Intelligence},
  year         = {2025},
  howpublished = {\url{https://github.com/bar181/ross-agi-score}},
  note         = {Version 1.0. Conceptual framework paper.}
}
