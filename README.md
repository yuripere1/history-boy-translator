# History Boy Translator

A tiny Streamlit web app that translates text into the custom "History Boy" texting voice.

## 1. Install

Python 3.10+ is recommended.

```bash
pip install -r requirements.txt
```

## 2. Add your API key

Mac/Linux:

```bash
export OPENAI_API_KEY="your_api_key_here"
```

Windows PowerShell:

```powershell
$env:OPENAI_API_KEY="your_api_key_here"
```

Or create a `.env`/secrets setup appropriate for your deployment. Do not commit your API key to GitHub.

## 3. Run

```bash
streamlit run app.py
```

Then open the local address Streamlit prints, usually:

`http://localhost:8501`

## Deploying

This can be deployed to Streamlit Community Cloud, another Python host, or run privately on your computer.

For a public deployment, store `OPENAI_API_KEY` in the hosting provider's secret/environment-variable settings rather than in the source code.

## Customizing

The full voice specification is in `SYSTEM_PROMPT` near the top of `app.py`. You can edit it to add more reference messages, names, preferred spellings, or additional style rules.
