# Ross AGI Score (RAS) Paper - Revision Plan 
## last updated: May 10, 2025

## ✅ **SECTION-BY-SECTION UPDATE OUTLINE**

---

### **1. Abstract**

*   **Update Needed:**
    *   [ ] Add a **clear problem statement**: What gap in AGI evaluation the RAS fills.
    *   [ ] Add 1–2 lines on **how RAS is constructed (15-level ACL + dimensions)**.
    *   [ ] Add a brief mention of **how RAS compares to frameworks like ARC-AGI and Levels-of-AGI**.
*   **Rationale:**
    Provides better context for readers skimming abstracts on arXiv. Currently it’s conceptually sound but not comparative or concrete enough.
*   **Status:** To Do
*   **Notes/Plan:**
    *   _Draft 1: [Your initial thoughts/draft for the revised abstract]_
    *   _Ensure word count remains appropriate for an abstract._

---

### **2. Introduction**

*   **Update Needed:**
    *   [ ] Include citations to **Levels of AGI (Morris et al., 2023/2024 - *confirm year and find formal citation*)** and **ARC-AGI (Chollet et al., 2024 - *confirm year and find formal citation*)** early in the background.
    *   [ ] Replace the current general narrative with a **tighter 3-paragraph layout**:
        *   (1) What AGI is and why we need better evaluations.
        *   (2) Current gaps in evaluation (benchmarks, imitation tests).
        *   (3) What RAS proposes and how this paper is structured.
*   **Rationale:**
    The current intro lacks an explicit roadmap and underspecifies novelty vs prior benchmarks.
*   **Status:** To Do
*   **Notes/Plan:**
    *   _Paragraph 1 Draft: [Focus on AGI definition and evaluation need]_
    *   _Paragraph 2 Draft: [Summarize gaps, referencing key existing methods]_
    *   _Paragraph 3 Draft: [Introduce RAS as solution, outline paper structure]_

---

### **3. Section 2: Background and Related Work**

*   **Update Needed:**
    *   [ ] Add a **dedicated paragraph comparing RAS to:**
        *   DeepMind’s Levels of AGI (Morris et al.)
        *   ARC-AGI (Chollet et al.)
        *   Chollet’s skill-acquisition efficiency definition (from original 2019 ARC paper)
        *   Universal Intelligence (Legg & Hutter)
        *   Conceptual tests (Coffee Test, etc.)
    *   [ ] Each comparison should clarify **what RAS shares and what it adds (novelty/differentiation).**
*   **Rationale:**
    Without situating RAS in the ecosystem of AGI evaluations, it may be viewed as reinventing the wheel.
*   **Status:** To Do
*   **Notes/Plan:**
    *   _For each comparison, identify 1-2 shared principles and 1-2 unique contributions of RAS._
    *   _Ensure this paragraph flows logically with the rest of Section 2._

---

### **4. Section 3: RAS Framework Overview**

*   **Update Needed:**
    *   [ ] **Define all cognitive dimensions** clearly, in a bullet list or table within this section or as a dedicated sub-section.
    *   [ ] Add **mathematical formula or scoring algorithm** (even pseudocode) showing how sub-scores on dimensions aggregate to an overall RAS ACL.
        *   _Example: Overall ACL = min(ACL_dim1, ACL_dim2, ..., ACL_dimN) if this is the "minimum profile requirements" approach._
    *   [ ] State clearly: Are all dimensions weighted equally? Can the weights be customized (and if so, how or is this future work)?
*   **Rationale:**
    For arXiv and reproducibility, a framework must be defined precisely enough for others to implement or understand its scoring logic.
*   **Status:** To Do
*   **Notes/Plan:**
    *   _List the 10 dimensions from the scorecard template here._
    *   _Draft pseudocode for the aggregation rule based on "minimum profile requirements."_
    *   _Address weighting explicitly._

---

### **5. Section 4: AGI Capability Levels**

*   **Update Needed:**
    *   [ ] This section is well-developed, but needs a **summary table** of all 15 levels with concise labels (e.g. ACL 1: Minimal Narrow AI, ACL 7: Early Emergent AGI, ACL 10: Full Human-Level AGI, ACL 15: Theoretical Maximum AGI).
    *   [ ] Add **cross-references to examples or behaviors** from Section 5 (Minimum Profile Requirements) or the (optional) worked example section, if added.
*   **Rationale:**
    While thorough, the section is long and could benefit from a visual index or executive summary for readers.
*   **Status:** To Do
*   **Notes/Plan:**
    *   _Create a two-column table: ACL Number | Concise Label & Brief Descriptor._
    *   _Review Section 5 and identify specific behavioral examples to cross-reference._

---

### **6. Section 5: Minimum Profile Requirements**

*   **Update Needed:**
    *   [ ] Add **bullet-point criteria** for each AGI stage (I–IV) aligned to the defined cognitive dimensions.
    *   [ ] Consider a **matrix table** (or adapt the existing bullet list into a more structured format):
        | Stage        | ACL Range | Minimum Score per Dimension (Conceptual) | Qualifying Behavior Examples (from Sec 4) |
        | ------------ | --------- | ---------------------------------------- | --------------------------------------- |
        | Stage I      | 1–6       | Fails to meet Stage II criteria          | e.g., Lacks cross-domain adaptability   |
        | Stage II     | ~7–9      | e.g., All core dimensions ≥ ACL 7, one ≥ ACL 8/9 | e.g., Independent learning, generalization |
        | Stage III    | 10        | All core dimensions ≥ ACL 10             | e.g., Robust human-level performance across tasks |
        | Stage IV     | 11–15     | All core ≥ ACL 10, ≥1 dimension > ACL 10 | e.g., Superhuman speed/accuracy/insight |
    *   [ ] Clarify if **all dimensions are equal gatekeepers** for stage advancement (the current text implies yes, but make it explicit).
*   **Rationale:**
    The stage classification needs a clearer operational checklist. A policy or safety analyst will want a clear “threshold” indicator.
*   **Status:** To Do
*   **Notes/Plan:**
    *   _Review the current descriptions for each stage and extract/formalize the bullet-point criteria per dimension._
    *   _Draft the matrix table._

---

### **7. Section 6: Future Work and Roadmap**

*   **Update Needed:**
    *   [ ] Condense slightly; restructure into **3 priority tiers**:
        *   Short-Term (e.g., test design, initial calibration studies, precise dimension definition)
        *   Mid-Term (e.g., open-source toolkit, broader validation studies, community feedback incorporation)
        *   Long-Term (e.g., policy integration, evaluation of new AI paradigms like multi-agent systems, advanced safety/alignment links)
    *   [ ] Reference any existing work or tangible assets (e.g., "The RAS Scorecard template presented in Appendix A serves as an initial basis for test suite design.").
*   **Rationale:**
    Helps arXiv readers and collaborators know what’s concrete now vs future aspiration.
*   **Status:** To Do
*   **Notes/Plan:**
    *   _Re-categorize current roadmap items into the three tiers._
    *   _Ensure language reflects a balance of ambition and current progress._

---

### **8. Section 7: Conclusion**

*   **Update Needed:**
    *   [ ] Tighten to 3–5 core contributions (bullet format is good).
    *   [ ] Restate **key limitations** explicitly (e.g., RAS is currently a conceptual framework, not yet empirically validated on a wide range of AI systems; test batteries are under development; direct measurement of safety/alignment is out of scope for RAS capability scores but synergistic).
*   **Rationale:**
    The conclusion is solid but should echo a more professional “Findings + Limitations + Call to Action” format.
*   **Status:** To Do
*   **Notes/Plan:**
    *   _Extract core contributions from the current conclusion._
    *   _Formulate 2-3 key limitations based on the current state and roadmap._

---

### **9. References**

*   **Update Needed:**
    *   [ ] Check every citation for accuracy (authors, year, title, publication venue), validity, and ensure working URL/DOI.
    *   [ ] Remove any overly informal references (e.g., blog posts, LinkedIn, unless they are the primary source for a specific, cited claim and properly archived/stable). *Self-correction: The current reference list is mostly academic; this is more a general reminder.*
    *   [ ] **Add (and cite in text where appropriate):**
        *   Formal citation for **Morris et al. (2023/2024)** for Levels of AGI (e.g., arXiv:2311.02462 if confirmed).
        *   Formal citation for **Chollet et al. (2024)** for ARC-AGI (if this is a new paper distinct from the 2019 ARC paper, find it. Otherwise, ensure the 2019 paper is appropriately discussed for ARC).
        *   **Wang, P. (e.g., 2008, 2009)** AGI evaluation surveys (Need to identify these specific surveys by Pei Wang or others if intended). If specific surveys aren't found, ensure the existing literature review covers the evolution of AGI evaluation thinking adequately.
*   **Rationale:**
    Some essential works in the AGI evaluation space might be missing or need updated citations for completeness and accuracy.
*   **Status:** To Do
*   **Notes/Plan:**
    *   _Systematically review each reference entry._
    *   _Research and add the missing key citations if they are indeed distinct and relevant works._

---

### **10. Optional: Add a Worked Example Section**

*   **Add New Section (Recommended):**
    **“Section X: Illustrative RAS Evaluation of a Hypothetical System”** – show a filled-out RAS scorecard (based on the template in Appendix A) for a hypothetical AI agent (e.g., "a current-generation advanced LLM" or "a hypothetical proto-AGI system").
    *   Provide brief justifications for the ACL scores assigned to each dimension for this hypothetical system.
    *   Show how the overall AGI Stage is derived.
*   **Rationale:**
    This gives a clear demonstration of RAS in action, solidifying its practical value and how the different components (dimensions, ACLs, minimum requirements, stages) interact.
*   **Status:** To Do (Consider for high impact)
*   **Notes/Plan:**
    *   _Develop a profile for a hypothetical AI (e.g., strong in language, moderate in reasoning, weak in embodiment)._
    *   _Fill out the scorecard template from Appendix A._
    *   _Write a brief narrative explaining the scoring and stage classification._

---

### **11. Appendix A: Ross AGI Scorecard Template**

*   **Update Needed:**
    *   [ ] Ensure the scorecard template from the separate file is included as Appendix A.
    *   [ ] Add a brief introductory sentence to the Appendix explaining its purpose.
    *   [ ] Clarify "Evaluation Basis (P1/P2)" in a footnote or introductory note within the appendix (e.g., P1=Direct Test Results, P2=Inferred from Documentation/Observed Behavior).
*   **Rationale:**
    The scorecard is a key practical output and should be formally included and briefly explained.
*   **Status:** To Do
*   **Notes/Plan:**
    *   _Copy template into Appendix._
    *   _Add explanatory note for P1/P2._

---

### **General Paper-Wide Considerations:**

*   [ ] **Consistency:** Ensure consistent terminology (e.g., "AGI Capability Levels" vs. "ACL bands") and formatting throughout.
*   [ ] **Clarity of Figures/Tables:** If new tables are added (summary of ACLs, matrix for stages), ensure they are clear, well-labeled, and referenced correctly in the text.
*   [ ] **"Release Date" Metadata:** Re-evaluate the "Release Date: May 11, 2025" vs. document date "May 11, 2024" for clarity.
*   [X] **"Table 1 (conceptually)" Reference:** Address the mention of "Table 1" in Section 3, either by removing it, adding a conceptual table, or rephrasing to point to the Appendix scorecard or the new ACL summary table. **Appendix A provided with supporting file**

