# RuSentiment

Проект по анализу русскоязычного датасета тональности [`MonoHime/ru_sentiment_dataset`](https://huggingface.co/datasets/MonoHime/ru_sentiment_dataset).

## Что сделано

- EDA текстовых данных.
- Тематическое моделирование через `NMF + TF-IDF`.
- Визуализация найденных тем.
- Обучение классификатора тональности: `TF-IDF + Logistic Regression`.
- Оценка качества модели и скорости инференса.
- CPU-оптимизация классификатора через ONNX Runtime.

## Результаты

- Test accuracy: `0.7575`
- Test macro F1: `0.7524`
- Test weighted F1: `0.7604`
- Test log loss: `0.5519`

## Файлы

- `ru_sentiment_solution.ipynb` — выполненный Jupyter notebook с решением.
- `ru_sentiment_logreg_classifier.onnx` — ONNX-версия обученного классификатора.

## Данные

Датасет не добавлен в репозиторий из-за большого размера. Скачать можно так:

```powershell
git lfs install
git clone https://huggingface.co/datasets/MonoHime/ru_sentiment_dataset
```

