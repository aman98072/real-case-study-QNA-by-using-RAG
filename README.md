## Quick Start

1. **Clone the repository**
2. **Create a virtual environment:**
   ```bash
   python -m venv .venv
   source .venv/Scripts/activate
   ```
3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```
4. **Start OpenSearch:**  
   ```
   Make sure your OpenSearch instance is running on `localhost:9200` (or update the connection settings in the code)

5. **Create `.env` file & Save API KEY**
   ```bash
   GEMINI_API_KEY=
   ```
6. **Ingest Chunks**
   ```bash
   python ingestion.py
   ```
7. **Run the app**
   ```bash
   python app.py
   ```

## Project Structure

- `app.py` – Main application entry point
- `chunking.py` – PDF and data chunking logic
- `generation.py` – RAG response generation
- `retrieval.py` – Search and retrieval utilities
- `ingestion.py` - Ingest Chunks to VectorDB
- `helper.py` – Supporting modules
