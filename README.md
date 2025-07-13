# LLM-judge-divergence-kaggle
# 🧠 LLM Judge Divergence – Kaggle Competition (Dec 2024 – Mar 2025)

Hi! This repo contains the code and notebook I used for the [Kaggle competition](https://www.kaggle.com/competitions/llms-you-cant-please-them-all), **“LLMs: You Can’t Please Them All”**. The challenge was to generate short essays (up to 100 words) that would **trigger disagreement among three LLM-based judges**, while still being fluent, readable, and relevant.

---

## 🧩 What Was the Task?

The competition asked participants to:
- Generate **100-word essays** based on given topic IDs.
- Maximize **horizontal** (judge disagreement on same essay) and **vertical** (one judge being inconsistent) divergence.
- Maintain **good English fluency**, **uniqueness**, and **natural style**.

There was no training data — just prompts and LLMs evaluating submissions behind the scenes.

---

## 🚀 My Approach

I built a prompt generation pipeline using Python and some reinforcement-inspired logic. Here’s what I focused on:

- ✅ Engineered prompts that balance **ambiguity**, **opinion**, and **clarity**.
- 🔁 Added **controlled randomness** and **topic diversity** (cultural, moral, abstract).
- ✂️ Pruned repetitive or weak outputs.
- 🧠 Tried to tap into **LLM sensitivities** like tone, word choice, and framing.

---

## 📁 Files & Structure

llm-judge-divergence/
│
├── llm_submission.ipynb # My main notebook to generate essays
├── input.csv # Topic IDs (from Kaggle)
├── submission.csv # Final output to upload to Kaggle
├── README.md # This file!


---

## ⚙️ How to Use This Notebook

1. Add the `input.csv` file from Kaggle (with prompt IDs like `prompt_1`, etc.).
2. Run the notebook `llm_submission.ipynb`.
3. It generates 100 essays (each under 100 words) and saves them to `submission.csv`.
4. You can then upload this file directly to the Kaggle competition page.

---

## 🧪 What I Learned

This competition was a really interesting test of:
- **Prompt engineering** without training data
- Understanding how **LLMs respond to ambiguity or subtle tone shifts**
- Thinking creatively while sticking to strict format rules

---

## 🧠 Future Improvements

If I revisit this, I'd like to:
- Add a scoring simulator to better guess divergence offline
- Try style-transfer techniques for more tone variation
- Integrate GPT-based generation for higher fluency control

---

## 🔗 Competition Link

👉 [LLMs: You Can’t Please Them All – Kaggle](https://www.kaggle.com/competitions/llms-you-cant-please-them-all)

---

Thanks for checking this out!  
If you're exploring prompt engineering, LLM behavior, or essay generation — I’d love to connect.
