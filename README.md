<<<<<<< HEAD
# Setup

## 1. Clone the Repository

```bash
git clone <your-repository-url>
cd <repository-name>
```

## 2. Create Virtual Environment

```bash
python -m venv .venv
```

### Windows

```bash
.venv\Scripts\activate
```

### Linux / macOS

```bash
source .venv/bin/activate
```

## 3. Install Dependencies

```bash
pip install -U langgraph langchain-groq python-dotenv langgraph-checkpoint-sqlite
```
or
```bash
pip install -r requirements.txt
```


## 4. Configure API Key

Create a `.env` file in the project root:

```env
GROQ_API_KEY=your_groq_api_key
```

The application loads it using:

```python
from dotenv import load_dotenv

load_dotenv()
```

## 5. Run the Notebook

Open the `.ipynb` file in VS Code or Jupyter and run the cells sequentially.

```bash
jupyter notebook
```

## 6. SQLite Database

The SQLite database is created automatically when running the checkpointing example:

```text
chatbot.db
```

Do **not** commit `.env` or `*.db` files to GitHub.

Recommended `.gitignore`:

```gitignore
.env
.venv/
__pycache__/
*.db
.ipynb_checkpoints/
```
=======
# handson_langraph
>>>>>>> 473774b7318a2af0c1aa05b9067264418dc90ecb
