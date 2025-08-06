# 📚 TextInova: AI-Powered Academic Text Toolkit

TextInova is an intelligent academic web application that integrates **Paraphrasing**, **Text Summarization**, and **Plagiarism Detection** into a single, user-friendly platform. Designed specifically for students, researchers, and content creators, TextInova ensures originality, clarity, and professionalism in writing tasks.

## 🔍 Features

### ✍️ Paraphrasing Tool
- **Model Used:** Pegasus (`tuner007/pegasus_paraphrase`)
- **Customization Filters:**
  - 🎓 Academic Filter
  - 👤 First Person Removal
  - 🔁 Active/Passive Voice Conversion

### 📝 Text Summarization
- **Models Used:** BART (abstractive), TF-IDF with cosine similarity (extractive)
- **Custom Options:**
  - Summary Type: `Abstractive / Extractive`
  - Tone: `Neutral / Formal / Informal`
  - Length: `Short / Medium / Long / Custom`

### 🔍 Plagiarism Detection
- **Intrinsic Plagiarism Detection:** Stylometric analysis via TF-IDF & cosine similarity
- **AI-Generated Text Detection:** RoBERTa-based classification

---

## 🚀 Technologies Used

| Component       | Technology        |
|----------------|-------------------|
| Frontend       | Streamlit         |
| Backend        | Flask             |
| NLP Models     | Pegasus, BART, RoBERTa |
| Libraries      | HuggingFace Transformers, NLTK, Scikit-learn, spaCy, PyMuPDF/pdfplumber |

---

## 🖥️ System Requirements

### Software:
- Python 3.9+
- Streamlit, Flask, Transformers, PyTorch/TensorFlow
- Compatible browsers: Chrome, Firefox, Edge

### Hardware:
- Recommended: 16GB RAM, SSD storage
- Optional GPU: NVIDIA GTX series or above

---

## 📂 Folder Structure

```bash
academic_app/
│
├── app.py                     # Main Streamlit app
├── paraphraser.py            # Paraphrasing logic
├── summarizer.py             # Summarization logic
├── plagiarism_checker.py     # Intrinsic plagiarism detection
├── ai_detector.py            # AI-generated text classifier
├── utils.py                  # Shared utility functions
├── models/                   # Stored pre-trained models or config
├── sample_files/             # Test .pdf/.docx files
├── requirements.txt          # Python dependencies
└── README.md                 # Project documentation
⚙️ Setup Instructions
Clone the repository

bash
Copy
Edit
git clone https://github.com/yourusername/textinova.git
cd textinova
Create virtual environment

bash
Copy
Edit
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate
Install dependencies

bash
Copy
Edit
pip install -r requirements.txt
Run the app

bash
Copy
Edit
streamlit run app.py


📄 How to Use
Upload or paste your text in the app.

Choose one or more tools:

Paraphraser: Select tone/style filters.

Summarizer: Pick type, tone, and length.

Plagiarism Checker: Scan for AI-generated or stylistically inconsistent content.

Review the generated output, compare with original, and export the results if needed.

🎯 Project Goals
Provide a one-stop platform for academic content processing.

Promote ethical writing by preventing plagiarism and over-reliance on AI.

Assist non-native English speakers and students in improving their writing clarity and tone.

👩‍💻 Developed By
Priya G S
Vaishnavi D
Preetham K 
Sudeep 
Department of Artificial Intelligence & Data Science,
K.S. School of Engineering and Management (KSSEM), Bengaluru
Academic Year: 2024–2025

📜 License
This project is part of an academic submission and is not licensed for commercial reuse without permission.
