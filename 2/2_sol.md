### 1. Which of the following is true?
- Extremistan has thin tails while Mediocristan has long tails  
- Mediocristan distributions are harder to predict than Extremistan  
- **In Extremistan, the total is determined by a few large events with tyranny of the accidental**  
- Extremistan has mild randomness while Mediocristan has wild randomness  

**Correct Response:**  
*In Extremistan, the total is determined by a few large events with tyranny of the accidental*  

**Reasoning:**  
Extremistan distributions (e.g., wealth, social media engagement) are dominated by extreme outliers that disproportionately influence the total, unlike Mediocristan (e.g., height, weight) where events cluster around the mean.

---

### 2. What is the key difference between covariate shift and concept shift in distribution shifts?
- Covariate shift changes P(y|x) while concept shift changes P(x)  
- **Covariate shift changes P(x) while P(y|x) remains constant, concept shift changes P(y|x) while P(x) remains constant**  
- Both change P(x) and P(y|x) simultaneously  
- Covariate shift affects labels while concept shift affects features  

**Correct Response:**  
*Covariate shift changes P(x) while P(y|x) remains constant, concept shift changes P(y|x) while P(x) remains constant*  

**Reasoning:**  
- **Covariate shift**: Input distribution (`P(x)`) changes (e.g., training on daylight images, testing on night images).  
- **Concept shift**: Input-output relationship (`P(y|x)`) changes (e.g., "spam" definition evolves over time).  

---

### 3. In the AugMix methodology, what is the primary advantage over uncontrolled random augmentations?
- **It uses skip connections to keep images recognizable while applying diverse augmentations**  
- It requires less computational power  
- It only applies single augmentations instead of multiple  
- It focuses on geometric transformations only  

**Correct Response:**  
*It uses skip connections to keep images recognizable while applying diverse augmentations*  

**Reasoning:**  
AugMix blends multiple augmentations via skip connections to preserve semantic content, improving robustness without distorting the original image beyond recognition.

---

### 4. In the context of adversarial attacks, what does "transferability" specifically refer to?
- The ability to transfer attacks from one domain to another  
- The ability to transfer defenses across different architectures  
- The ability to convert white-box attacks to black-box attacks  
- **The ability of adversarial examples crafted for one model to work on other models**  

**Correct Response:**  
*The ability of adversarial examples crafted for one model to work on other models*  

**Reasoning:**  
Transferability exploits shared vulnerabilities across models, enabling black-box attacks without knowledge of the target model's architecture.

---

### 5. Black Swan lies in which of the following categories?
- Known Knowns  
- Known Unknowns  
- Unknown Knowns  
- **Unknown Unknowns**  

**Correct Response:**  
*Unknown Unknowns*  

**Reasoning:**  
Black Swan events (e.g., pandemics, financial crashes) are unforeseen and unpredictable, falling into the "unknown unknowns" category.

---

### 6. Which of the following are valid approaches for defending against adversarial attacks? (Select all that apply)
- **Data augmentation techniques**  
- **Adversarial training using adversarial examples during training**  
- **Using more data and larger models**  
- Reducing model complexity to avoid overfitting  
- Adversarial pretraining on larger datasets like ImageNet  

**Correct Responses:**  
*Data augmentation techniques, Adversarial training using adversarial examples during training, Using more data and larger models*  

**Reasoning:**  
- **Data augmentation** and **adversarial training** improve robustness by exposing models to varied/perturbed inputs.  
- **Larger models/data** enhance generalization. Reducing complexity or pretraining alone are insufficient defenses.

---

### 7. In the RLHF optimization objective, why is a KL-divergence penalty term added to the reward maximization?
- To prevent the model from generating repetitive outputs  
- **To ensure the model stays close to the original pretrained model**  
- To improve the computational efficiency of the training process  
- To increase the diversity of generated samples  

**Correct Response:**  
*To ensure the model stays close to the original pretrained model*  

**Reasoning:**  
The KL penalty prevents the policy from deviating too far from the pretrained model's behavior, avoiding extreme/unintended outputs.

---

### 8. What does "reward hacking" specifically refer to in the context of RLHF?
- Humans providing incorrect feedback to manipulate the system  
- External attackers compromising the reward model  
- The reward model overfitting to the training data  
- **The model finding ways to maximize the reward function without achieving the intended behavior**  

**Correct Response:**  
*The model finding ways to maximize the reward function without achieving the intended behavior*  

**Reasoning:**  
Reward hacking occurs when models exploit loopholes in the reward function (e.g., generating verbose text to maximize "engagement").

---

### 9. Identify the equations that can lead to a long-tailed distribution.
- **Idea * student * resources * time**  
- Idea * student + resources * time  
- Idea + student + resource + time  
- Idea - student * resource - time  

**Correct Response:**  
*Idea * student * resources * time*  

**Reasoning:**  
Multiplicative interactions (e.g., `A*B*C`) create power-law/long-tailed distributions, where outliers dominate the total.

---

### 10. What is the primary advantage of using pairwise comparisons over direct scalar ratings in human feedback collection?
- Pairwise comparisons are faster to collect  
- They require fewer human annotators  
- **Human judgments are noisy and miscalibrated, but pairwise comparisons are more reliable**  
- They provide more granular feedback information  

**Correct Response:**  
*Human judgments are noisy and miscalibrated, but pairwise comparisons are more reliable*  

**Reasoning:**  
Pairwise comparisons reduce noise by focusing on relative judgments (e.g., "A is better than B"), which humans perform more consistently than absolute scoring.

---

### 11. What is a major challenge with using a single reward function in RLHF?
- It is computationally expensive to optimize  
- **It cannot represent a diverse society of humans**  
- It requires too much training data  
- It is unstable during training  

**Correct Response:**  
*It cannot represent a diverse society of humans*  

**Reasoning:**  
A single reward function oversimplifies human values, which are inherently pluralistic and context-dependent.

---

### 12. What is Direct Preference Optimization (DPO) equivalent to in the context of RLHF component removal?
- RLHF - Human Feedback  
- **RLHF - Reward Model**  
- RLHF - RL  
- RLHF - Policy Optimization  

**Correct Response:**  
*RLHF - Reward Model*  

**Reasoning:**  
DPO eliminates the need for an explicit reward model by directly optimizing preferences, simplifying the RLHF pipeline.
