# Hi, I'm Nazeer

Applied Data Science & AI student at **Breda University of Applied Sciences** (Netherlands).
I build end-to-end machine learning systems: from training and evaluating models to packaging, deploying and monitoring them.

I care about measuring things properly. Every project below reports results on a fixed evaluation protocol, compares against baselines, and explains what did not work as well as what did.

## Featured projects

### [Plant Root Phenotyping](https://github.com/nazeer-idris/plant-root-phenotyping)
**Computer vision, robotics and MLOps** · built with NPEC (Netherlands Plant Eco-phenotyping Centre)

U-Net root segmentation on petri-dish images, root-tip localisation, and a simulated liquid-handling robot that inoculates the tips on its own. The same pipeline is served as a production platform with an API, dashboard and drift monitoring.

- Root segmentation: **validation F1 0.873** (own U-Net)
- Auto-tuned PID controller: **100%** of 105 reaches settled within 1 mm, median error 0.14 mm
- SAC + HER reinforcement learning agent and a hybrid RL → PID controller, benchmarked on identical tasks
- Autonomous inoculation: **5/5** root tips hit, mean droplet error **0.13 mm**
- Team platform (my parts): Docker deployment, PostgreSQL + Alembic, confidence-based drift detection, Azure cost analysis

`TensorFlow` `OpenCV` `Stable-Baselines3` `PyBullet` `FastAPI` `PostgreSQL` `Docker` `Azure ML` `Next.js`

### [Speech Translation & Emotion Classification](https://github.com/nazeer-idris/speech-translation-emotion-classification)
**NLP pipeline: Arabic speech → English text → 7 emotions**

Whisper transcribes Arabic audio, NLLB-200 translates it, and a fine-tuned DeBERTa-v3-large labels the emotion of every sentence. Uncertain predictions are flagged for human review. Includes a Gradio demo, CLI, tests, error analysis and explainability study.

- Compared 15 models on one test set, from TF-IDF + Naive Bayes to Llama 3.3 70B
- Shipped model raised macro F1 from **0.374 → 0.499** over the previous off-the-shelf classifier
- Seven prompt engineering iterations on Llama 3.2 3B and 3.3 70B
- Translation benchmark across four NLLB-200 checkpoints (BLEU up to 39.8)
- Found and fixed a label-mapping bug that stopped the original classifier from ever predicting *neutral* or *disgust*

`PyTorch` `Hugging Face Transformers` `Whisper` `NLLB-200` `DeBERTa` `Gradio` `pytest`

## Currently working on

- **AI museum guide** for Stedelijk Museum Breda, built on BrabantCloud heritage data (team project, data science role)
- **Workflow automation** with n8n and LLM APIs, such as a Telegram calorie tracker that logs meals to Google Sheets using image recognition

## Tech stack

**Languages:** Python, SQL, TypeScript
**ML & DL:** PyTorch, TensorFlow / Keras, scikit-learn, Hugging Face Transformers, OpenCV
**LLMs & NLP:** Llama, Whisper, NLLB-200, Claude API, Gemini API, prompt engineering, XAI
**Reinforcement learning:** Stable-Baselines3, Gymnasium, PyBullet
**Backend & data:** FastAPI, PostgreSQL, SQLAlchemy, Alembic
**MLOps & tooling:** Docker, Azure ML, MLflow, Airflow, GitHub Actions, pytest, Ruff, uv
**Automation:** n8n

## Contact

- LinkedIn: [nazeer-idris](https://www.linkedin.com/in/nazeer-idris/)
- Email: [nazeer.idris@outlook.com](mailto:nazeer.idris@outlook.com)
