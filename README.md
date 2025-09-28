Heart Disease Prediction – ML Project
📌 О проекте
Цель проекта – предсказать наличие сердечно-сосудистых заболеваний на основе набора признаков пациентов.
Проект демонстрирует полный цикл работы с данными: EDA → предобработка → моделирование → оценка качества → интерпретация признаков.
🗂 Датасет
Источник: heart.csv (реальные медицинские данные)
Размер: 1190 строк, 12 признаков
Признаки:
Числовые: age, resting_bp_s, cholesterol, max_heart_rate, oldpeak
Категориальные: sex, chest_pain_type, fasting_blood_sugar, resting ecg, exercise_angina, st_slope
Целевая переменная: target
0 = Нет заболевания
1 = Есть заболевание
🔍 Exploratory Data Analysis (EDA)
Построены гистограммы, scatterplots и heatmap корреляций.
Наиболее сильные признаки, коррелирующие с болезнью: st_slope, exercise_angina, chest_pain_type.
⚙️ Предобработка данных
Числовые признаки: масштабирование через StandardScaler.
Категориальные признаки: кодирование через OneHotEncoder.
Использован ColumnTransformer и Pipeline → чистый и масштабируемый подход.
🧩 Модели
Logistic Regression
Accuracy: ~0.90
Recall (для класса больных): 0.93
Random Forest Classifier
Accuracy: 0.95
Precision / Recall / F1-score: ≈ 0.95–0.96
Модель показывает отличный баланс между классами и высокую точность.
📊 Feature Importance (Random Forest)
Топ-10 важнейших признаков:
st_slope
exercise_angina
chest_pain_type
oldpeak
Барчарт показывает, какие признаки реально влияют на предсказание болезни.
📝 Метрики оценки
Model	Accuracy	Precision	Recall	F1-score
Logistic Regression	0.90	0.90	0.93	0.91
Random Forest	0.95	0.95	0.96	0.96
💡 Выводы
Random Forest — сильнее Logistic Regression по точности и сбалансированности.
Проект демонстрирует умение:
Работать с реальными данными
Проводить EDA и визуализацию
Строить ML модели и оценивать их
Интерпретировать результаты через feature importance
Проект можно использовать как учебный портфель для стажировок в ML / Data Science.