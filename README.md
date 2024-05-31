# article_emotional_classification
Структура ноутбуков:
1) znanie_text_preprocess.ipynb - первичная предобработка текстов (удаление стоп-слов, вики-разметки, ссылок, телефонных номеров)
2) gemini_ai_labeling.ipynb - разметка и парсинг требуемых лексических конструкций из предобработанных текстов (с помощью промпта и API gemini-1.5-pro)
3) znanie_training_on_labeled_data.ipynb - постобработка текста, подключение векторной БД для дальнейшего использования RAG-системы и обучения моделей для предсказания тональности текстов (ruBERT-tiny, catboost с перебором гиперпараметров через optuna)
