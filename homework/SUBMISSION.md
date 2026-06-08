# Submission

Заполните файл перед отправкой PR в репозиторий-образец `MaratNotes/rag-tutorial`.

## Ссылка на репозиторий с заданием

- Repo URL: https://github.com/Marrrik/rag_hw

## Автор

- Старченко Марк Альбертович БАСБ251
ник: Marrrik

## Комментарий

- **Что реализовано:** учебный RAG по теме «Космос и астрономия». Полный offline-pipeline:
  сбор корпуса из русской Википедии → ingestion → chunking → TF-IDF индекс → retrieval
  (cosine top-k) → demo-ответ с источниками и отказом → Streamlit UI.
- **Данные:** 1319 статей русской Википедии → 3802 чанка (планеты, звёзды, галактики,
  кометы, космические аппараты и миссии), собраны воспроизводимо через MediaWiki API
  (`scripts/prepare_datasets.py`), без Kaggle API и авторизации.
- **Что улучшено:** реализованы 7 из 8 направлений (см. `IMPROVEMENTS.md`), кроме
  векторной БД: эмбеддинги (sentence-transformers), гибридный поиск, reranking
  (cross-encoder), LLM-генерация (OpenAI-совместимая, с фолбэком), оценка качества
  (Hit@k/MRR/refusal-rate), доработка Streamlit UI, data pipeline + версионирование.
- **Тесты:** `uv run pytest tests/ -v` — 25 тестов зелёные.
