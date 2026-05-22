# Документация проекта

Индекс **планирования и разработки**. Запуск, тесты и demo-вопросы — в [корневом README.md](../README.md).

## Документы

| Документ | Содержание |
|----------|------------|
| [00_project_idea.md](00_project_idea.md) | Идея, цель, данные |
| [vision.md](vision.md) | Техническое видение, стек MVP |
| [conventions.md](conventions.md) | Правила для code-ассистента |
| [tasklist.md](tasklist.md) | Итерационный план разработки |
| [workflow.md](workflow.md) | Как выполнять итерации |
| [DATA.md](DATA.md) | Источники данных, что индексируем |

## Порядок чтения

1. [00_project_idea.md](00_project_idea.md) — зачем проект
2. [vision.md](vision.md) — стек и границы
3. [tasklist.md](tasklist.md) + [workflow.md](workflow.md) — как строили MVP
4. [DATA.md](DATA.md) — откуда данные и что в индексе

## Стек MVP (фактический)

| Компонент | Выбор |
|-----------|-------|
| Поиск | TF-IDF + cosine similarity |
| Индекс | `vectorizer.pkl` + `matrix.npz` (локально) |
| UI | Streamlit |
| Ответ | Demo-режим без внешней LLM |

Подробности — [vision.md](vision.md).
