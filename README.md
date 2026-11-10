# 🎓 Smart Subject Tutor (v1.0 — Open-Source RAG)

An open-source, zero-API-key **Retrieval-Augmented Generation (RAG)** tutor built in GitHub Codespaces that adapts explanations across four pedagogical styles.

## 🏗️ v1.0 Architecture
- **Subject Knowledge Base:** `data/subject_notes.md`
- **Embedding Model:** `sentence-transformers/all-MiniLM-L6-v2` ($\vec{v} \in \mathbb{R}^{384}$)
- **Vector Database:** `ChromaDB` using Cosine Similarity ($\cos \theta$)
- **Open-Source LLM:** `Qwen/Qwen2.5-0.5B-Instruct` (CPU-optimized)
- **Adaptive Styles:** ELI10 Analogy, Exam Topper, Socratic Professor, Practical Engineer

## 🚀 How to Run in GitHub Codespaces
```bash
python3 -m venv .venv
source .venv/bin/activate
pip install torch --index-url https://download.pytorch.org/whl/cpu
pip install -r requirements.txt
streamlit run app.py

2. Stop the terminal server by pressing `Ctrl + C` in the terminal, or click the **Source Control** icon on the left sidebar of Web VS Code (`Ctrl + Shift + G`).
3. Verify that only your $5$ project files appear under **Changes**:
   * `.gitignore`
   * `README.md`
   * `requirements.txt`
   * `data/subject_notes.md`
   * `rag_engine.py`
   * `app.py`
4. Type the commit message:
   ```text
   feat(v1): launch open-source RAG smart subject tutor with adaptive teaching styles
