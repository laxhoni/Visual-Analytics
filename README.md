PROYECTO-FINAL-VISUAL-ANALYTICS/
│
├── data/                   # <--- ¡OJO! NO subir archivos grandes aquí (ver punto 3)
│   ├── 01_raw/             # Datos originales (all-the-news.csv filtrado)
│   ├── 02_processed/       # Datos con métricas NLP calculadas (csv limpio)
│   └── 03_synthetic/       # Datos generados por IA (output de GPT)
│
├── notebooks/              # Tu laboratorio de pruebas (sucio y rápido)
│   ├── 1_data_filtering.ipynb     # Filtrado pre-2020 y muestreo
│   ├── 2_ai_generation.ipynb      # Script para llamar a OpenAI API
│   ├── 3_feature_extraction.ipynb # Cálculo de métricas (Lexical diversity, etc)
│   └── 4_model_training.ipynb     # Entrenamiento XGBoost + Análisis SHAP
│
├── src/                    # Código fuente limpio y reutilizable
│   ├── __init__.py
│   ├── nlp_utils.py        # Funciones para limpiar texto y calcular métricas
│   └── model_utils.py      # Funciones para cargar/guardar modelos
│
├── app/                    # La aplicación Streamlit (El entregable final)
│   ├── main.py             # Punto de entrada de la app
│   ├── pages/              # Páginas extra si las necesitáis
│   └── utils_viz.py        # Funciones específicas para gráficos
│
├── models/                 # Modelos entrenados guardados
│   ├── xgboost_classifier.pkl
│   └── shap_explainer.pkl
│
├── reports/                # Documentación
│   └── final_report.pdf    # El informe de 3 páginas (para el 08/12)
│
├── .gitignore              # ¡CRÍTICO! (Ver abajo)
├── requirements.txt        # Lista de librerías (streamlit, shap, xgboost...)
└── README.md               # Explicación de cómo ejecutar el proyecto
