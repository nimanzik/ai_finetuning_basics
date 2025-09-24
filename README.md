# Fine-Tuning Open-Weight Models: A Hands-On Deep Learning Primer

## Welcome!

In this workshop, we’ll go hands-on with **fine-tuning small open-weight models** and, along the way, pick up deep learning foundations every builder should know.

We’ll:  
- 🧑‍🏫 Learn when to system prompt vs. fine-tune  
- ⚖️ Compare small open-weight models vs. large API models  
- 📉 Interpret training metrics and read **loss curves** like a practitioner  
- 🧠 Understand embeddings, parameter sizes, and model architecture basics  
- 🛠️ Fine-tune a **270M open-weight model** in Colab  
- 📊 Evaluate whether your fine-tune is really working  

All running in **Google Colab** with free GPU/TPU access — no setup headaches and no prior deep learning experience required.

---

This workshop was inspired in part by a talk given by **Ravin Kumar** during [Hugo Bowne-Anderson’s course, *Building LLM-Powered Applications for Data Scientists and Software Engineers*](https://maven.com/s/course/d56067f338).

Next cohort starts **November 3** — use code `LLM10` for 10% off (valid until Nov 2, 2025)!

---

## 🛠 Workshop Flow

### ✅ Phase 0: Fast setup (Colab-first)

- Open the provided **Colab notebook** and select a GPU/TPU runtime.  
- Verify you can load and prompt a small **~270M parameter** open-weight model.  
- (Optional) Try locally if you have Apple Silicon or an NVIDIA GPU; CPU is possible but very slow.  

---

### ✅ Phase 1: Prompting vs. Fine-Tuning

- Start with **system prompting** to push the model’s behavior.  
- See where prompting breaks (easy to override, inconsistent).  
- Discuss when it’s worth updating weights instead of crafting prompts (think: changing the model’s “prior”).  

---

### ✅ Phase 2: Hands-On Fine-Tuning (soccer vs. football + alien speech)

You’ll actually train a **~270M open-weight model** to specialize.

- **Goal 1**: make the model consistently handle “**soccer**” vs. “**football**” distinctions  
  (e.g., region-aware wording, rules/terms, examples).  
- **Goal 2**: fine-tune the model on “**alien speech**” so it can translate synthetic alien-language snippets into human-readable text.  

**Workflow in the notebook:**  
- Prepare/inspect a small task-specific dataset.  
- Run the fine-tuning loop.  
- Save the updated weights/checkpoints.  
- Compare **base vs. fine-tuned** model outputs on test prompts.  

---

### ✅ Phase 3: Deep Learning Essentials (practitioner view)

- Learn how to interpret **training curves** and **loss metrics**.  
- Explore embeddings, parameter sizes, and model architecture basics.  
- Debug common issues (overfitting, underfitting, unstable training).  

---

### ✅ Phase 4: Evaluation

- Go beyond vibes: measure whether your fine-tune is really working.  
- Test on held-out prompts and structured evals.  
- Revisit both fine-tune examples:  
  - ⚽🏈 **Soccer vs. Football** — does the model consistently disambiguate?  
  - 👽 **Alien Speech** — does the model reliably translate alien → human text?  

---

## 🚀 Getting Started

1. Open the provided **Colab notebooks** — no installation required.  
2. Follow along with the code in your browser.  
3. For power users: you can run locally with Apple or NVIDIA GPUs (optional).  

---

## ⚡ Requirements
- ✅ Runs in **Colab** out of the box (free GPU/TPU).  
- ⚡ Optional: run locally with your own Apple/NVIDIA GPU (CPU possible but very slow).  
- 📦 No prior deep learning experience required — just curiosity.  


## 📂 Repository Structure
