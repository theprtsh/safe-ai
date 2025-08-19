### 1. What is considered an ideal Stereotype Score (ss)?
- **0%**
- 25%
- 50%
- 75%

**Correct Response:**  
*0%*  

**Reasoning:**  
A Stereotype Score (ss) measures the proportion of stereotypical associations in model outputs. An ideal score is 0%, indicating no stereotypical bias.

---

### 2. What does SEAT stand for?
- Standard Evaluation Assessment Test
- Semantic Evaluation Annotation Test
- Structured Embedding Accuracy Test
- **Sentence Embedding Association Test**

**Correct Response:**  
*Sentence Embedding Association Test*  

**Reasoning:**  
SEAT is a bias evaluation method inspired by the Implicit Association Test (IAT), measuring associations between concepts (e.g., gender-career) in sentence embeddings.

---

### 3. In counterfactual data augmentation (CDA), what is altered to rebalance the corpus?
- Sentence Length
- Syntax
- **Bias attribute words**
- Vocabulary complexity

**Correct Response:**  
*Bias attribute words*  

**Reasoning:**  
CDA generates counterfactuals by swapping bias attributes (e.g., gender: "nurse" → "male nurse") to create balanced data and reduce spurious correlations.

---

### 4. Which characteristic makes a language model more likely to generate gender-neutral responses in text-to-text tasks? (Select all that apply.)
- **Training on diverse and balanced datasets.**
- Use of bias-specific adapter modules.
- **Conditioning outputs on explicit gender tokens.**
- Reliance on pretrained token embeddings without fine-tuning.

**Correct Responses:**  
*Training on diverse and balanced datasets., Conditioning outputs on explicit gender tokens.*  

**Reasoning:**  
- **Diverse datasets** reduce inherent biases.  
- **Explicit gender tokens** (e.g., [MASK]) allow controlled, neutral generation.  
Adapters alone may not suffice, and pretrained embeddings often contain biases.

---

### 5. Which toolkit is used to add programmable guardrails to LLM-based conversational applications like ChatGPT?
- GPT-4
- NVIDIA NeMo
- **CoDi**
- MAFIA

**Correct Response:**  
*CoDi*  

**Reasoning:**  
CoDi (Compositional Diffusion) is a toolkit for integrating safety guardrails (e.g., content filters, rule-based constraints) into LLM workflows.

---

### 6. Which of the following is the correct formula for Pointwise Mutual Information (PMI)?
- PMI(wi,wj)=log2N⋅c(wi,wj)c(wi)2⋅c(wj)2
- PMI(wi,wj)=log2c(wi)⋅c(wj)N⋅c(wi,wj)
- **PMI(wi,wj)=log2N⋅c(wi,wj)c(wi)⋅c(wj)**
- PMI(wi,wj)=log2c(wi,wj)N⋅c(wi)⋅c(wj)

**Correct Response:**  
*PMI(wi,wj)=log2N⋅c(wi,wj)c(wi)⋅c(wj)*  

**Reasoning:**  
PMI quantifies the association between words. The standard formula is:  
`PMI(wi, wj) = log2( [c(wi,wj) * N] / [c(wi) * c(wj)] )`,  
where `c` is count and `N` is total word pairs.

---

### 7. ‘Useful fairness’ couples which of the following? (Select all that apply.)
- **Context awareness**
- Bias Score
- **STS task performance**
- Dataset diversity

**Correct Responses:**  
*Context awareness, STS task performance*  

**Reasoning:**  
"Useful fairness" emphasizes that debiasing should not degrade utility (e.g., performance on Semantic Textual Similarity (STS) tasks) and should be context-aware.

---

### 8. What is the key architectural idea behind the MAFIA model for effective debiasing?
- **Fusing bias-specific adapters while keeping the base model the same.**
- Replacing all model weights with debiased adapters.
- Dynamically routing inputs based on detected bias type.
- Using GANs to hallucinate fair outputs.

**Correct Response:**  
*Fusing bias-specific adapters while keeping the base model the same.*  

**Reasoning:**  
MAFIA uses lightweight, composable adapters for each bias type (e.g., gender, race), enabling targeted debiasing without altering the base model.

---

### 9. Which of the following is true about proprietary models?
- **They are more neutral compared to CoDi and other open source models.**
- They are less neutral compared to CoDi and other open source models.
- They have more bias than CoDi and other open source models.
- They have the same neutrality as CoDi and other open source models.

**Correct Response:**  
*They are more neutral compared to CoDi and other open source models.*  

**Reasoning:**  
Proprietary models (e.g., GPT-4) often undergo extensive debiasing and alignment, making them more neutral than many open-source alternatives.

---

### 10. Which of the following are benchmark datasets commonly used to measure bias in language models? (Select all that apply.)
- **Stereoset**
- **CrowS-Pairs**
- ImageNet
- **Bias-STS-S**
- SQuAD

**Correct Responses:**  
*Stereoset, CrowS-Pairs, Bias-STS-S*  

**Reasoning:**  
- **Stereoset** and **CrowS-Pairs** measure social biases.  
- **Bias-STS-S** evaluates bias in Semantic Textual Similarity.  
ImageNet and SQuAD are for vision and QA, not bias-specific.

---

### 11. What is ‘gender-bleaching’ in the context of VLMs?
- Improving the quality of input images.
- Turning all people in the input images white.
- Enhancing gender-specific features in input images.
- **Removing/Obscuring visual cues related to gender in input images.**

**Correct Response:**  
*Removing/Obscuring visual cues related to gender in input images.*  

**Reasoning:**  
Gender-bleaching techniques (e.g., blurring hairstyles, clothing) minimize gender signals in visual data to reduce bias in Vision-Language Models (VLMs).

---

### 12. Why might a single adapter for all bias types (like iDEBall) fail?
- **Cannot effectively debias across all categories.**
- Trains slower than other models.
- Requires more input data.
- Does not understand contextual information.

**Correct Response:**  
*Cannot effectively debias across all categories.*  

**Reasoning:**  
Different biases (e.g., gender, race) require distinct mitigation strategies. A single adapter lacks specialization, leading to inadequate debiasing.
