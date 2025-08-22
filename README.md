# 🌸 VirtueGPT

**From the Gita, Ramayana, and beyond – a philosophical guide to a virtuous life.**

VirtueGPT is a **Streamlit-powered conversational AI** that provides philosophical guidance and reflection based on the timeless wisdom of the **Bhagavad Gita**, the **Ramayana**, and the teachings of great Indian philosophers such as **Swami Vivekananda**. It is designed as a **compassionate, philosophical guide** to help users explore questions about life, duty, purpose, and inner peace through the lens of virtue.

-----

## 📖 About The Project

In a world full of distractions, **virtue** stands as a timeless compass. VirtueGPT was built to bridge **ancient philosophy** with **modern AI**, offering a safe, reflective, and empathetic space for **self-discovery and wisdom**. Unlike simple Q\&A bots, VirtueGPT provides **philosophical insights** inspired by scripture and profound thinkers, encouraging deeper reflection rather than quick answers.



-----

## ✨ Key Features

  * **Conversational AI Interface:** An interactive, minimalist chat interface powered by Streamlit.
  * **Gita + Ramayana + Philosophy Dataset:** Responses are grounded in the wisdom of the Bhagavad Gita, the Ramayana, and the public domain works of Indian philosophers like Swami Vivekananda.
  * **Virtue-Centered Guidance:** Answers are contextualized around core virtues like truth, compassion, courage, and wisdom.
  * **Multilingual Verse Display:** View verses in Sanskrit, Telugu, and English.
  * **Voice Support:** Ask questions via microphone input (speech-to-text) and listen to the AI's responses via text-to-speech playback.
  * **Empathetic Persona:** The AI maintains a calm, reflective, and non-preachy tone.

-----

## 🛠️ Tech Stack & Architecture

  * **Frontend:** Streamlit
  * **LLM:** Gemma:2b (via Ollama)
  * **Embedding Model:** TensorFlow Hub (Universal Sentence Encoder)
  * **Vector Database:** ChromaDB
  * **Speech-to-Text:** OpenAI Whisper / SpeechRecognition
  * **Text-to-Speech (TTS):** pyttsx3 / gTTS
  * **Core Architecture:** Retrieval-Augmented Generation (RAG)

### 🔎 Workflow

1.  **Query Embedding:** The user's query is converted into a vector embedding.
2.  **Semantic Search:** ChromaDB retrieves the most relevant verses or philosophical texts.
3.  **Context Assembly:** A context-rich prompt is created with the retrieved verse and commentary.
4.  **Thoughtful Response:** The Gemma LLM generates calm, reflective guidance.
5.  **Voice Output:** The answer is optionally spoken aloud via TTS.

-----

## 🚀 Getting Started

### Prerequisites

  * Python 3.9+
  * Ollama installed and running
  * Microphone enabled

### Installation

```bash
git clone https://github.com/your-username/VirtueGPT.git
cd VirtueGPT
```

Create and activate a virtual environment:

```bash
python -m venv virtue
# Windows PowerShell
.\virtue\Scripts\Activate.ps1
# macOS / Linux
source virtue/bin/activate
```

Install requirements:

```bash
pip install -r requirements.txt
```

Download the LLM:

```bash
ollama pull gemma:2b
```

Add the datasets to your project directory. These are JSON files containing the knowledge base:

  * `gita_knowledge_base.json`
  * `ramayana_knowledge_base.json`
  * `philosophy_quotes.json`

Run the app:

```bash
streamlit run app.py
```

Access the app in your browser at `http://localhost:8501`.

-----

## 🗺️ Roadmap & Future Plans

  - [x] Add Bhagavad Gita + Ramayana verses
  - [x] Integrate Swami Vivekananda’s writings (public domain)
  - [x] Add voice input + output support
  - [ ] Expand to all \~700 Gita verses
  - [ ] Add full Ramayana coverage
  - [ ] Incorporate other Indian philosophical schools (Vedanta, Yoga, Nyaya, etc.)
  - [ ] Build a full Telugu-first immersion mode
  - [ ] Create a mobile-friendly PWA version
  - [ ] Implement a user feedback loop to rate responses

-----

## 🤝 How to Contribute

We warmly welcome contributions to this project. You can help by:

  * **Expanding the Knowledge Base:** Add more verses, translations, or public domain philosophy texts.
  * **Writing Commentaries:** Add modern commentaries in English or Telugu.
  * **Code Enhancements:** Optimize the RAG system, improve the speech modules, or polish the UI.
  * **Providing Feedback:** Share your ideas, report bugs, or suggest new features.
  * **Improving Documentation:** Enhance the clarity of guides and instructions.

-----

## 🙏 Acknowledgements

  * **Bhagavad Gita:** Public domain translations.
  * **Ramayana:** Public domain translations.
  * **Swami Vivekananda:** Collected works in the public domain.
  * **Open-source contributors** and **spiritual knowledge keepers** who have preserved and shared this wisdom.
