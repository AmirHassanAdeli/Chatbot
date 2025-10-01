📖 RAG-based QA Chatbot (Persian)

This project is a simple Retrieval-Augmented Generation (RAG) chatbot designed for answering questions in Persian based on a given document.
It combines semantic search with generative AI to provide accurate and context-aware answers.

🚀 Features
	•	📚 Splits a text document into chunks for efficient retrieval
	•	🔎 Uses SentenceTransformers (MiniLM Multilingual) for semantic embeddings
	•	⚡ Stores and searches embeddings with FAISS (vector database)
	•	🤖 Generates answers with DeepSeek Qwen-1.5B language model
	•	📝 Answers in fluent Persian (فارسی روان)
	•	🎯 Returns “در متن پاسخی پیدا نشد.” if the answer is not in the text

🛠️ Tech Stack
	•	Python 3
	•	SentenceTransformers
	•	FAISS
	•	Transformers (HuggingFace)
	•	DeepSeek Qwen Model
	•	PyTorch

📂 Project Structure

.
├── processed_text.txt     # Input document (plain text)
├── chatbot.ipynb          # Main notebook with code
├── requirements.txt       # Python dependencies
└── README.md              # Project documentation

⚙️ Installation

Clone the repository and install dependencies:

git clone https://github.com/AmirHassanAdeli/Chatbot
cd your-repo
pip install -r requirements.txt

▶️ Usage
	1.	Put your text inside processed_text.txt.
	2.	Run the notebook chatbot.ipynb.
	3.	Start asking questions in Persian, e.g.:

❓ سؤال شما: نقش دانشگاه در توسعه علمی کشور چیست؟
🤖 چت‌بات: دانشگاه نقشی کلیدی در پرورش نیروی انسانی متخصص و تولید علم دارد.

🧩 Example Workflow
	•	Load and chunk text → Encode with MiniLM → Store in FAISS → Retrieve relevant chunks
	•	Provide chunks + user query to DeepSeek Qwen → Generate concise Persian response

🔮 Future Improvements
	•	Add support for streaming answers
	•	Deploy as a web app (e.g., with FastAPI or Streamlit)
	•	Add database persistence for embeddings
	•	Improve prompt engineering for better control

