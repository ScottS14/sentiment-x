# Sentiment-X — Cross-Domain Sentiment Classification

Predict positive/negative sentiment that *generalises* across **Amazon**, **Yelp**, and **IMDB** reviews.

| Phase | ETA |
|-------|-----|
| Data ingest + TF-IDF baseline | Week 1 (21 – 27 Jul) |
| DistilBERT + LoRA fine-tune   | Week 2 |
| Domain-adaptive MLM + error analysis | Week 3 |
| Streamlit dashboard & v1.0 release   | Week 4 (by 17 Aug) |

Quick-start:

```bash
uv venv .venv
uv pip install -r requirements.txt
bash scripts/fetch_data.sh          # downloads + preprocesses
python -m src.models.train_tfidf
