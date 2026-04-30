## **InsightRank: XAI-Based Resume Auditor**

**InsightRank** is an Explainable AI (XAI) platform designed to bridge the gap between traditional black-box recruitment tools and transparent career guidance[cite: 1]. It evaluates resume alignment with job descriptions using semantic understanding rather than simple keyword matching[cite: 1].

---

### **Key Features**
*   **Semantic Matching**: Uses `all-MiniLM-L6-v2` to identify conceptual matches between resumes and job requirements[cite: 1].
*   **Requirement-Level Explainability**: Breaks down the job description to show exactly which resume sections support each specific requirement[cite: 1].
*   **Skill Gap Analysis**: Automatically identifies missing skills and provides direct links to personalized learning resources (Coursera/Udemy)[cite: 1].
*   **Transparent Scoring**: Converts complex AI similarity scores into intuitive, human-readable percentages using a calibrated sigmoid function[cite: 1].

---

### **Technical Architecture**
*   **Frontend**: Built with **Streamlit** for rapid, interactive deployment[cite: 1].
*   **NLP Pipeline**: Utilizes **pypdf** for text extraction and a **Sliding Window** strategy for context-aware chunking[cite: 1].
*   **Core Model**: A **Bi-Encoder** Sentence Transformer optimized for CPU speed and real-time inference[cite: 1].
*   **Training Objective**: Employs a hybrid loss function ($0.8 \times MSE + 0.2 \times CrossEntropy$) to balance precise scoring with categorical accuracy[cite: 1].

---

### **Why InsightRank?**
Unlike traditional ATS systems that penalize formatting and hide their logic, InsightRank focuses on **Post-hoc Explainability**[cite: 1]. It answers the "Why?" behind every score, helping candidates understand their standing and how to improve[cite: 1].
