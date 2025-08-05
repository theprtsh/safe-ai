### 1. What is the definition of “Machine Unlearning”?
- **Removing the influences of training data from a trained model**  
- The ability of a machine learning model to adapt to new data  
- A technique used to compress machine learning models  
- The ability of a machine learning model to learn a variety of data  

**Correct Response:**  
*Removing the influences of training data from a trained model*  

**Reasoning:**  
Machine unlearning focuses on eliminating the impact of specific data points from a trained model, often for privacy, compliance, or safety reasons (e.g., GDPR "right to be forgotten").  

---

### 2. What might be some types of information that one might want to remove from model data? (Select all that apply.)
- **Private data**  
- **Toxic or unsafe content**  
- Accurate information  
- Model hyperparameter settings  
- **Stale knowledge**  

**Correct Responses:**  
*Private data, Toxic or unsafe content, Stale knowledge*  

**Reasoning:**  
- **Private data**: To comply with privacy laws (e.g., GDPR).  
- **Toxic content**: To mitigate harmful model outputs.  
- **Stale knowledge**: To update outdated information (e.g., obsolete medical guidelines).  

---

### 3. What is GDPR’s Article 17 about in the context of Machine Learning?
- Right to be remembered  
- Right to be modified  
- Right to be distributed  
- **Right to be forgotten**  

**Correct Response:**  
*Right to be forgotten*  

**Reasoning:**  
GDPR Article 17 mandates that individuals can request deletion of their personal data, necessitating machine unlearning techniques in ML systems.  

---

### 4. What are the steps in the SISA approach?
- Sampled, Isolated, Stopped, Aggregated  
- Sharded, Imitate, Sliced, Annotated  
- **Sharded, Isolated, Sliced, Aggregated**  
- Sampled, Imitate, Stopped, Annotated  

**Correct Response:**  
*Sharded, Isolated, Sliced, Aggregated*  

**Reasoning:**  
SISA (Sharded, Isolated, Sliced, Aggregated) is a framework for efficient unlearning by partitioning data into shards, training submodels in isolation, and aggregating results.  

---

### 5. What is Membership Inference Attack (MIA) used for?
- To train LLMs faster  
- To improve the model’s robustness  
- To remove accurate data  
- **To classify between training and unseen data**  

**Correct Response:**  
*To classify between training and unseen data*  

**Reasoning:**  
MIA determines whether a specific data point was part of a model’s training set, posing privacy risks (e.g., exposing sensitive training data).  

---

### 6. What is the role of differential privacy?
- To improve model accuracy  
- To make the model forget everything  
- **To make models indistinguishable with/without certain data points**  
- To speed up training time  

**Correct Response:**  
*To make models indistinguishable with/without certain data points*  

**Reasoning:**  
Differential privacy adds noise to ensure statistical queries/results don’t reveal whether any individual’s data was included.  

---

### 7. Which benchmarks are used to evaluate unlearning in LLMs? (Select all that apply.)
- **TOFU**  
- GLUE  
- **WMDP**  
- GUIDE  

**Correct Responses:**  
*TOFU, WMDP*  

**Reasoning:**  
- **TOFU** (Task-forgetful Unlearning): Evaluates forgetting specific training tasks.  
- **WMDP** (World Model Disinformation Prevention): Assesses removal of hazardous knowledge.  
- GLUE/GUIDE are not unlearning benchmarks.  

---

### 8. Case: A hospital shares aggregate statistics to protect patient identities. Which form of unlearning is this?
- Exact unlearning  
- **Unlearning via differential privacy**  
- Just ask for unlearning  
- Empirical Unlearning  

**Correct Response:**  
*Unlearning via differential privacy*  

**Reasoning:**  
Aggregate statistics with noise (e.g., counts, averages) align with differential privacy, preventing re-identification of individuals.  

---

### 9. Which isn’t a type of graph unlearning?
- Node unlearning  
- Edge unlearning  
- **Label unlearning**  
- Node feature unlearning  

**Correct Response:**  
*Label unlearning*  

**Reasoning:**  
Graph unlearning typically involves nodes, edges, or features—not labels, which are properties of nodes/edges rather than structural elements.  

---

### 10. Which methods are used for Node unlearning? (Select all that apply.)
- **GraphEraser**  
- GUIDE  
- Projector  
- **GraphdEditor**  
- **GNNDelete**  
- MEGU  

**Correct Responses:**  
*GraphEraser, GraphdEditor, GNNDelete*  

**Reasoning:**  
These methods specifically target node removal in graphs:  
- **GraphEraser**: Retrains affected subgraphs.  
- **GraphdEditor**: Updates embeddings locally.  
- **GNNDelete**: Uses influence functions.  

---

### 11. What are “hidden representations”?
- The final model outputs  
- Raw training data stored in memory  
- **Intermediate activation vectors captured during model execution**  
- The model’s loss values during training  

**Correct Response:**  
*Intermediate activation vectors captured during model execution*  

**Reasoning:**  
Hidden representations are the transformed inputs at intermediate layers of a neural network, encoding features used for predictions.  
