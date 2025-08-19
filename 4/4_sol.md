### 1. As per the lecture, in the context of Machine Learning, what is the definition of ‘bias’?
- Systematic deviation from rationality and judgement.
- Systematic error in the collection, analysis, or interpretation of data.
- **Systematic favoritism or discrimination towards certain groups/outcomes.**
- Systematic behaviour when solving complex tasks.

**Correct Response:**  
*Systematic favoritism or discrimination towards certain groups/outcomes.*  

**Reasoning:**  
In ML, bias often refers to systematic unfairness that advantages or disadvantages specific groups (e.g., racial or gender bias in predictions), not just statistical error.

---

### 2. Why did Microsoft’s Tay chatbot become offensive shortly after it was launched?
- **It learned toxic behaviour from user interactions on Twitter.**
- It was hacked by a rival company.
- It was trained on outdated information.
- It was programmed to be controversial for publicity.

**Correct Response:**  
*It learned toxic behaviour from user interactions on Twitter.*  

**Reasoning:**  
Tay was designed to learn from user interactions, but malicious users exploited this by feeding it offensive content, causing it to generate harmful responses.

---

### 3. As per the lecture, which of the following is a/are a category of bias? (Select all that apply.)
- **Gender**
- **Race**
- Scientific Facts
- **Profession**
- Currency exchange rates

**Correct Responses:**  
*Gender, Race, Profession*  

**Reasoning:**  
Bias in ML often manifests along social dimensions like gender, race, and profession (e.g., stereotyping certain jobs), not factual or economic domains.

---

### 4. According to the ML Pipeline, what may be a source of bias? (Select all that apply.)
- **Annotators beliefs**
- Hardware used for computation
- Balanced dataset
- **Biased training data**

**Correct Responses:**  
*Annotators beliefs, Biased training data*  

**Reasoning:**  
- **Annotators beliefs**: Human labelers may inject subjective biases.  
- **Biased training data**: Historical or unrepresentative data perpetuates biases.  
Hardware and balanced datasets typically reduce, not cause, bias.

---

### 5. What does the Legal Safety Score (LSSβ) represent?
- The model's ability to predict legal outcomes based solely on accuracy.
- **A metric combining fairness and accuracy using a β-weighted harmonic mean.**
- A score based on the usage of legal jargon for marginalized groups.
- An evaluation metric used to define how well a model understands legal jargon.

**Correct Response:**  
*A metric combining fairness and accuracy using a β-weighted harmonic mean.*  

**Reasoning:**  
LSSβ balances fairness (e.g., equitable outcomes across groups) and accuracy, avoiding over-reliance on either alone.

---

### 6. What do LLMs use to prevent harmful outputs?
- Data augmentation
- **Guardrails**
- Faster GPUs
- Dropout layers

**Correct Response:**  
*Guardrails*  

**Reasoning:**  
Guardrails are filters or rules (e.g., keyword blocking, toxicity classifiers) that intercept and mitigate harmful LLM outputs before they reach users.

---

### 7. Which of the following is true about bias?
- It never exists.
- It sometimes exists.
- It only exists in American-created models.
- **It always exists.**

**Correct Response:**  
*It always exists.*  

**Reasoning:**  
Bias is inherent in all data and models due to historical, societal, or sampling limitations—it can be mitigated but never fully eliminated.

---

### 8. A researcher selects only ideal images for testing, ignoring diverse cases. Which type of bias is this?
- Reporting bias
- Sampling bias
- **Experimenter’s bias**
- Historical bias

**Correct Response:**  
*Experimenter’s bias*  

**Reasoning:**  
Experimenter’s bias occurs when researchers consciously or subconsciously influence results (e.g., cherry-picking data that supports their goals).

---

### 9. What is the issue with evaluating models only based on accuracy?
- Accuracy only reflects hardware performance.
- **Accuracy doesn’t reveal bias.**
- Accuracy checks for fairness.
- Accuracy changes the labelling.

**Correct Response:**  
*Accuracy doesn’t reveal bias.*  

**Reasoning:**  
High accuracy can mask biased performance (e.g., a model excelling on majority groups but failing on minorities), so fairness metrics are crucial.

---

### 10. Why might using Western-aligned datasets be problematic for the Indian demographic?
- The datasets are too large which may slow down training time.
- They are written in a different language.
- **They don’t reflect Indian social/societal norms.**
- They contain too many low-resolution images.

**Correct Response:**  
*They don’t reflect Indian social/societal norms.*  

**Reasoning:**  
Western datasets often encode cultural assumptions (e.g., names, traditions) that don’t generalize to India, leading to poor performance or bias.

---

### 11. What is a ‘stereotype’?
- A factual statement that applies to all humans.
- A scientifically proven characteristic.
- A legal rule used to govern a society.
- **A widely held belief about some group/entity.**

**Correct Response:**  
*A widely held belief about some group/entity.*  

**Reasoning:**  
Stereotypes are oversimplified generalizations (e.g., "all engineers are introverts") that can be perpetuated by ML models if trained on biased data.

---

### 12. What does the CrowS-Pairs dataset contain?
- **Pairs of sentences that differ only in minimally distant social bias.**
- Dialogues between humans and a chatbot.
- Pairs of biased and unbiased images.
- Code snippets with and without bugs.

**Correct Response:**  
*Pairs of sentences that differ only in minimally distant social bias.*  

**Reasoning:**  
CrowS-Pairs tests for social bias (e.g., gender, race) via sentence pairs where only the sensitive attribute changes (e.g., "He is a nurse" vs. "She is a nurse").

---

### 13. What is sampling bias?
- When historical data reflects inequalities that existed in the world at that time.
- When data is collected from a completely random and diverse group.
- **If proper randomization is not used during data collection.**
- When a model builder keeps training a model until it produces a result that aligns with their original hypothesis.

**Correct Response:**  
*If proper randomization is not used during data collection.*  

**Reasoning:**  
Sampling bias arises when data isn’t representative of the target population (e.g., surveying only urban users for a rural application).
