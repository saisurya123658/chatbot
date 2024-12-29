
# NLP Chatbot with Streamlit

This project implements a Natural Language Inference (NLI) chatbot using the Hugging Face `transformers` library and deploys it via Streamlit.

## Features
- Performs text classification based on NLI.
- User-friendly interface built with Streamlit.
- Real-time analysis of sentence pairs.

## Requirements
Ensure you have the required dependencies by installing from the `requirements.txt`:

```bash
pip install -r requirements.txt
```

## How to Run
1. Clone the repository:
```bash
git clone <repo-url>
cd chatbot-nli
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Run the Streamlit app:
```bash
streamlit run chatbot.py
```

4. Open the provided URL (e.g., `http://localhost:8501`) to access the chatbot.

## Project Structure
```
.
├── chatbot.py               # Main Streamlit app
├── requirements.txt         # Dependencies
├── README.md                # Project documentation
└── __pycache__              # Auto-generated compiled files (after running chatbot.py)
```

## How It Works
- The chatbot uses `facebook/bart-large-mnli` for NLI.
- Users input two sentences to check entailment.
- The model returns if one sentence entails the other, is neutral, or contradicts.

## Example
```
Sentence 1: A man is eating.
Sentence 2: Someone is having lunch.
Result: Entailment
Confidence: 0.95
```

## Notes
- Make sure to have `streamlit` and `transformers` installed.
- Modify `chatbot.py` to customize behavior or UI.

## License
This project is open-source under the MIT license.
