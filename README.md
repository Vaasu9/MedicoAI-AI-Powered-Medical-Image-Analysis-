# 🩺 MedicoAI: AI-Powered Medical Image Analysis Tool

MedicoAI is an intelligent, agent-powered medical imaging analysis tool built using **Agentic AI**, **Google Gemini multimodal models**, and **Streamlit**. This project allows users to upload medical images (e.g., X-rays, MRIs, CT scans), and receive a **structured, expert-level diagnostic report**, complete with a **patient-friendly explanation** and **research-backed insights**.

---

## 🚀 Features

- 🔬 **Agentic AI Analysis**: Uses a custom AI agent powered by Google Gemini and Agno SDK to interpret medical images.
- 🧠 **Multimodal Input**: Supports vision + text inputs for in-depth medical reasoning.
- 📸 **Image Preprocessing**: Automatically resizes and prepares uploaded images for analysis.
- 📄 **Detailed AI Report**: Includes image type, key findings, diagnosis, simplified explanation, and medical references.
- 🔎 **Web Search Integration**: Leverages DuckDuckGo tools to fetch the latest treatment protocols and research.
- 🖥️ **Interactive Streamlit UI**: Clean and responsive frontend for uploading images and viewing results.

---

## 🧠 Powered By

| Technology         | Description                                      |
|--------------------|--------------------------------------------------|
| [Agno SDK](https://pypi.org/project/agno/)       | Agent-based AI framework for reasoning and tool use. |
| Google Gemini 2.0  | Multimodal LLM (text + image).                  |
| DuckDuckGo Tools   | Real-time research queries for references.       |
| Streamlit          | Python web app framework for UI.                |
| Pillow (PIL)       | Image preprocessing and format handling.         |

---

## 📷 Supported Modalities

- X-ray
- MRI
- CT Scan
- Ultrasound
- Other standard diagnostic image formats (JPG, PNG, BMP, etc.)

---

## 📁 Project Structure


---

## 🧪 How It Works

1. **User uploads a medical image** via the Streamlit interface.
2. **Image is preprocessed** and passed to a multimodal AI agent.
3. **Agent analyzes the image** using Gemini + DuckDuckGo tools and a structured prompt.
4. **AI generates a detailed report** including diagnosis, key findings, and simplified explanation.
5. **UI displays the report** for medical professionals or patients.

---

## ⚙️ Installation

### 🔧 Prerequisites
- Python 3.8+
- Google Gemini API Key

### 📦 Setup Instructions

```bash
# 1. Clone the repo
git clone https://github.com/yourusername/MedicoAI.git
cd MedicoAI

# 2. Create a virtual environment (optional but recommended)
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# 3. Install dependencies
pip install -r requirements.txt

# 4. Set your Google API key
export GOOGLE_API_KEY="your_gemini_api_key"  # Or set it inside app.py

# 5. Run the Streamlit app
streamlit run app.py
