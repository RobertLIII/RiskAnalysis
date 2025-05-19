# Risk Summary Assistant with LLM

This prototype extracts and summarizes risk factors from SEC filings or other financial disclosures using a language model (LLM) pipeline. The tool provides both a high-level executive summary and a ranked list of top risks, streamlining a time-intensive aspect of financial analysis.

## 🔍 Overview

- **Input**: Raw or lightly preprocessed risk disclosure text (e.g., from 10-K filings).
- **Output**: 
  - Executive-level risk summary
  - Top 5 risk factors (ranked by significance)
- **Model**: GPT-based LLM (via OpenAI API)
- **Use case**: Analyst productivity aid, due diligence support, portfolio risk scan

## 🧠 Key Features

- Chunked document ingestion and summarization
- Customizable LLM prompts for modularity
- Separation of summary logic from formatting logic
- Basic security consideration notes for future integration
- Easily extendable for front-end interfaces or dashboards

## 🛠 Technologies Used

- Python (Colab environment)
- OpenAI GPT-4 API
- HTML export for front-end or stakeholder-friendly sharing

## 🧪 Demo

Demo and write-up available at:  
👉 [https://intelligenciaexmachina.com/risk-summary-assistant-with-llm/](https://intelligenciaexmachina.com/risk-summary-assistant-with-llm/)

## 🧱 Folder Structure

```
/RiskSummaryAssistant/
├── risk_summary_generator.py # Main logic
├── notebook.ipynb # Walkthrough and code demo
├── example_inputs/ # Sample risk sections
├── html_exports/ # Optional rendered outputs
└── README.md
```

## 🚧 Known Limitations

- Prompt injection risks exist if deployed as-is in public environments
- Assumes relatively clean input text (e.g., OCR noise not addressed)
- Not fine-tuned for domain-specific legal or regulatory language edge cases

## 📌 Next Steps / Extensions

- Integrate UI for broader usability (internal dashboards or client portals)
- Include entity-level risk tagging and filtering
- Automate document scraping and preprocessing from EDGAR

## 🛡 Disclaimer

This project is a personal prototype created for educational and portfolio purposes. It is not affiliated with or intended to represent any company or brand. All content is illustrative only.
