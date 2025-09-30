# Fine-Tuning Open-Weight Models: A Hands-On Deep Learning Primer

## Welcome!

In this workshop, we’ll go hands-on with **fine-tuning small open-weight models** and, along the way, pick up deep learning foundations every builder should know.

We’ll:
- 🧑‍🏫 Learn when to system prompt vs. fine-tune
- ⚖️ Compare small open-weight models vs. large API models
- 📉 Interpret training metrics and read **loss curves** like a practitioner
- 🧠 Understand embeddings, parameter sizes, and model architecture basics
- 🛠️ Fine-tune a **270M open-weight model** in Colab
- 📊 Evaluate whether your fine-tune is really working (with both classic metrics and LLM-as-a-Judge)

All running in **Google Colab** with free GPU access: no setup headaches and no prior deep learning experience required.

---

This workshop was inspired in part by a talk given by **Ravin Kumar** during [Hugo Bowne-Anderson’s course, *Building LLM-Powered Applications for Data Scientists and Software Engineers*](https://maven.com/s/course/d56067f338).

Next cohort starts **November 3** — use code `LLM10` for 10% off (valid until Nov 2, 2025)!

---

## 🛠 Workshop Flow

This workshop is broken down into three hands-on Colab notebooks. Start with the first and work your way through!

### 01_Zero_to_Prompts.ipynb: The "Before" Picture ([Colab notebook here](https://colab.research.google.com/drive/1J2i45upTf-S3uvPetrpenvME-MRKfOq5?usp=sharing))

First, we'll set up our environment and get a feel for the base model, `Gemma-270M`. We'll test its out-of-the-box capabilities on our two workshop tasks using only prompting, establishing a baseline and seeing where it falls short. This notebook answers the question: *Why do we need to fine-tune?*

- ✅ **Setup**: Load the model in Colab and connect to a free GPU.
- 🤔 **Prompting**: Test the model on two tasks:
    1.  **Football Classification**: Can it tell Australian (AFL) from American (NFL) teams?
    2.  **Alien Speech**: Can it role-play as a quirky alien NPC from a video game?
- 📉 **Baseline**: See the limits of prompting and why we need a better way to change model behavior.

---

### 02_Finetune_for_Classification_Football.ipynb: Your First Fine-Tune ([Colab notebook here](https://colab.research.google.com/drive/1gDwOhRFTpljxClx1p6oEEpOFUnrigqgv?usp=sharing))

Here, you'll execute your first fine-tune. We’ll focus on the structured **football classification** task. You'll learn the complete workflow: preparing a dataset, running the training loop, and evaluating the results with hard numbers. This is where you'll learn the core mechanics of training.

- 🗂️ **Data Prep**: Convert a simple list of teams into a conversational training dataset.
- ⚙️ **Training**: Use the Hugging Face `SFTTrainer` to fine-tune the model.
- 📈 **Deep Learning Essentials**: Learn to interpret **training and validation loss curves** to see if your model is actually learning.
- 🎉 **Evaluation**: Re-run our test and see the dramatic improvement in classification accuracy.

---

### 03_Finetune_for_Style_Alien_NPC.ipynb: Fine-Tuning for Persona ([Colab notebook here](https://colab.research.google.com/drive/17ymVtMtyzYlIc3k8ACtoEaFXUATUvObJ?usp=sharing))

Now we'll tackle a more creative task: teaching the model to adopt the **alien speech** persona. Simple accuracy doesn't work here, so we'll fine-tune for style and explore more advanced, qualitative evaluation techniques.

- 👽 **Stylistic Fine-Tuning**: Train the model on dialogue to make it adopt a unique, consistent persona.
- 🎯 **Good Overfitting**: See how "overfitting" can be a desirable outcome for locking in a specific character.
- ⚖️ **LLM-as-a-Judge**: When a simple metric won't do, we'll explore how to use another LLM to evaluate our model's stylistic consistency.

---

## 🚀 Getting Started

1.  Clone this repository or download the files.
2.  Open the `notebooks` directory.
3.  Start with `01_Zero_to_Prompts.ipynb` in Google Colab and follow the instructions inside.
4.  Proceed through the notebooks in order. Enjoy!

---

## ⚡ Requirements

- ✅ Runs in **Google Colab** out of the box (free GPU access recommended).
- 📦 No prior deep learning experience required: just curiosity.
- 🔑 A free [Hugging Face account](https://huggingface.co/join) is needed to download the Gemma model.

---
