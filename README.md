# Юлия Гаврилова

**Data Scientist** | Студентка 4 курса СПбГЭТУ «ЛЭТИ», специальность «Искусственный интеллект»

---

## Обо мне

Специализируюсь на работе с LLM: fine-tuning открытых моделей через LoRA/QLoRA, построение RAG-систем, оценка качества генерации, снижение галлюцинаций. Уверенно владею Python для ML (pandas, numpy, scikit-learn, PyTorch, CatBoost/XGBoost/LightGBM), имею опыт работы в Linux. Готова к экспериментам с генеративными моделями и решению нестандартных задач на стыке NLP и продакшн-разработки.

- Образование: СПбГЭТУ «ЛЭТИ», факультет компьютерных технологий и информатики, специальность «Информатика и вычислительная техника. Искусственный интеллект» (2023–2027), средний балл 4.7.
- Ключевые дисциплины: машинное обучение, нейронные сети, анализ данных, математическая статистика, базы данных, SQL.
- Английский язык: B2.

---

## Контакты

- Email: yuliya.gavrilova070705@gmail.com
- Telegram: @yrwqqy

---

## Навыки и технологии

**Языки и фреймворки:**  
Python (pandas, numpy, scikit-learn, PyTorch, transformers, FastAPI), SQL (PostgreSQL, оконные функции, CTE), PySpark.

**LLM и обработка естественного языка:**  
LoRA/QLoRA, instruction-style fine-tuning, prompt engineering (few-shot), работа с открытыми моделями (Qwen2.5), RAG (retrieval, chunking, reranking), FAISS, Qdrant, LangChain, LangGraph, LLM API (YandexGPT, Mistral AI), оценка качества (LLM-as-Judge, RAGAS, BLEU, ROUGE, BERTScore).

**Классическое машинное обучение:**  
Градиентный бустинг (LightGBM, XGBoost, CatBoost), логистическая регрессия, метрики (ROC-AUC, F1, Precision, Recall), SHAP-интерпретация.

**Инструменты и инфраструктура:**  
Git, Docker, Linux, Jupyter, FastAPI, MLflow (в процессе изучения).

---

## Проекты

Ниже представлены ключевые проекты. Код и детали – в соответствующих репозиториях.

### 1. Графовый пайплайн авторазметки обращений (LangGraph + RAG + LLM-as-a-Judge)
AI-агент для автоматической классификации пользовательских обращений по категории, срочности и тональности. Граф состояний на LangGraph с узлами RAG-поиска (FAISS), генерации через YandexGPT, оценки через LLM-as-a-Judge (Mistral AI) и ручной верификации. Достигнуты метрики: категория – accuracy 0.88, macro F1 0.86; срочность – 0.98; тональность – 0.94. Решение упаковано в Docker с FastAPI.  
→ [Ссылка на репозиторий](https://github.com/yuliagavrilova1111/langgraph-annotation)

### 2. AI-ассистент (RAG-бот) – пайплайн генерации ответов с источниками
Полный RAG-пайплайн: загрузка PDF, чанкинг, эмбеддинги SciRus-tiny, поиск в Qdrant, генерация через YandexGPT. Эксперименты с размером чанков. Оценка качества: BLEU, ROUGE, BERTScore F1 > 0.86, а также RAGAS (Faithfulness, Answer Relevancy, Context Precision). Вывод источников. Асинхронная обработка через aiogram 3.x, Docker, Yandex Cloud API.  
→ [Ссылка на репозиторий](https://github.com/yuliagavrilova1111/exam-rag-bot)

### 3. Гибридная авторазметка медицинских сущностей (Hybrid NER Extractor)
Дообучение Qwen2.5-0.5B с QLoRA в комбинации с spaCy для извлечения сущностей (PATIENT, DOCTOR, DRUG, DISEASE). Сгенерировано 600 синтетических примеров через YandexGPT. Эксперименты с рангом LoRA. Macro F1 > 0.9. FastAPI-сервис, тесты, Docker.  
→ [Ссылка на репозиторий](https://github.com/yuliagavrilova1111/hybrid-ner-extractor)

### 4. ML-детектор тональности
Дообучение ruBERT на 12 399 отзывах банков (banki.ru) для бинарной классификации. Тренировочный пайплайн на PyTorch. Macro F1 = 0.96. FastAPI-сервис с пакетной обработкой, логирование в SQLite, Docker, тесты.  
→ [Ссылка на репозиторий](https://github.com/yuliagavrilova1111/bank-sentiment-bert-service)

### 5. Прогнозирование дефолта и стресс-тестирование (Home Credit, Kaggle)
Обработка 8 таблиц через PySpark, создание 40+ признаков. Сравнение LightGBM, XGBoost, CatBoost и нейросети – лучшая CatBoost (ROC-AUC = 0.78, F1 macro = 0.627). SHAP-интерпретация, стресс-тестирование (рост среднего PD на 22.9%). FastAPI-микросервис.  
→ [Ссылка на репозиторий](https://github.com/yuliagavrilova1111/credit-risk-prediction)

---

## Статистика GitHub

[![Статистика GitHub](https://github-readme-stats.vercel.app/api?username=yuliagavrilova1111&show_icons=true&theme=default)](https://github.com/yuliagavrilova1111)
