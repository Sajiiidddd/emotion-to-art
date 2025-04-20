# 🎨 Picasso: Emotion-to-Art Generator  
### *"Your Inner Echoes"*

**Picasso** is an end-to-end deep learning pipeline that transforms human emotions into expressive AI-generated art. It combines advanced **emotion classification**, **prompt generation**, **image synthesis**, and **creative interpretation** using large language models to bring your inner feelings to life — visually and poetically.

---

## 🌈 Project Highlights

🔹 SBERT-based multi-label emotion classifier  
🔹 Fine-tuned on GoEmotions, DailyDialog, and EmpatheticDialogues  
🔹 Emotion-enhanced prompts using the NRC-VAD Lexicon  
🔹 Art generation via **Stable Diffusion XL Base**  
🔹 Artwork interpretation using **Gemini 1.5 Pro** API  
🔹 Designed to work seamlessly in **Google Colab**

---

## 🧠 Model Architecture

| Component            | Description                                                                 |
|----------------------|-----------------------------------------------------------------------------|
| **Text Encoder**      | [`all-MiniLM-L6-v2`](https://huggingface.co/sentence-transformers/all-MiniLM-L6-v2) |
| **Art Generator**     | `stabilityai/stable-diffusion-xl-base-1.0`                                 |
| **Emotion Datasets**  | GoEmotions, DailyDialog, EmpatheticDialogues, NRC-VAD Lexicon              |
| **LLM Interpreter**   | Google Gemini 1.5 Pro                                                       |

---

## ⚙️ Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/Sajiiidddd/emotion-to-art.git
cd emotion-to-art
```
### 2. Install Dependencies
```bash
pip install -r requirements.txt
```
### 3. Setup .env for API Keys
Create a .env file in the root directory and add the following:

```bash
HUGGINGFACE_TOKEN=your_huggingface_token_here
GEMINI_API_KEY=your_gemini_api_key_here
Important: Never hardcode your API keys. Keep them in .env and make sure .env is listed in .gitignore.
```

### 🚀 How to Use (Google Colab)
Open the notebook.ipynb file in Google Colab.

Upload your .env file securely when prompted.

Execute each cell in order to:

Load or train the SBERT emotion classifier

Generate emotional predictions from input text

Convert emotions into prompts

Generate art using Stable Diffusion XL

Interpret the artwork using Gemini


### 🔐 .gitignore Included
The repository includes a .gitignore that excludes:

API keys (.env)

Datasets and outputs

Model weights and checkpoints

System and cache files

Virtual environments and logs

### 📦 requirements.txt
All required packages are listed in requirements.txt. Install them using:

```bash
pip install -r requirements.txt
Main dependencies:

transformers, sentence-transformers, datasets

diffusers, torch, accelerate

google.generativeai, python-dotenv

scikit-learn, matplotlib, tqdm
```

🔮 Future Roadmap

🎙️ Add voice and facial emotion detection

🌐 Real-time webcam + audio feedback

🧠 Personalized art style adaptation

💻 Deploy as an interactive web app

### 🧑‍🎨 Creator
Sajid Tamboli 
LinkedIn • GitHub • Portfolio

### 📄 License
This project is licensed under the MIT License.



