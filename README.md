# 🧠 Second Brain (Python & JavaScript)

📌 What This Project Does

This project is an AI-powered Life Decision Simulator built to help recent graduates and young adults with career life decisions by showing scores, multi-dimensional graph, AI reasoning etc. I created it with AI assistance to act as a realistic, safety-first simulator. It takes human traits (like your burnout level, cash savings, risk tolerence etc) and calculates how these align across 8 different life tracks (like starting a buisness, going to grad school) all at the same time.

To keep it realistic, we built our data from trusted foundations:

1. The Synthetic Base: we generated a core dataset of 5,000 completely synthetic young-adult profiles across 8 different life tracks.
2. The Economic Floor (U.S. BLS 2023): Real, verified salary baselines and unemployment patterns.
3. Real Socioeconomic Benchmarks: 13,268 historical young-adult data records extracted directly from the UCI Adult Census Dataset.
4. The Final Balance Split: An 80% Training / 20% Testing split applied across an integrated 8,333-row master data matrix (a 60/40 blend of real census rows and diverse profile simulations).

Instead of relying completely on a single algorithm, we created a heterogeneous ensemble:
1. Random Forest Regressor (30% weight) - To capture sharp, non-linear feature interactions. 
2. Gradient Boosting (30% weight) - To minimize predictive errors sequentially and to increase accuracy.
3. Multi-Output deep neural network - To understand how different parts of your life affect each other, instead of looking at them one by one.
4. Decision Confidence Scorer - To check if a path is actually a good match and to stop the AI from giving a misleading recommendation.
5. Groq LLaMa 3.3 70B Layer - A linguistic mmodel that translates cold numbers into actionable data figures and writes an action plan.

📊 Results

We validated our AI performance using standard matrics (RMSE and R2 score). We ran 50 simulations (Monte Carlo Variance) for every career path and found out the best case and worst case scenarios to show risk and here are our scores:
1. Prediction accuracy - Our ensemble got an R2 of 0.80 and RMSE of 0.64 which shows that it reliably indentifies patterns.
2. Risk mapping - It marks stable paths (like bootcamps) and risky paths (like startup) which helps users see the dangers before going forward.
3. Safety Guard - Our decision confidence scorer has a very low error rate of 0.18 MAE.

🛠️ Tech Stack
1. Core modeling stack - Random forest, Gradient Boosting and Multi Output DNN
2. Explainability pipeline - SHAP (Shapley Additive Explanations) isolates and score the exact weight of each input.
3. AI Reasoning Layer - Groq LLaMA 3.3 70B
4. Platform - VSCode
5. Frontend - HTML5 dashboard style with CSS grid layout
6. API Framework - FastAPI / Flask REST API

🚀 How to Run
1. You need your Groq and Ngrok active API key.
2. Put the Groq API key in Cell 10 and Ngrok API key in cell 11 (REPLACE_WITH_YOUR_GROQ_API_KEY and REPLACE_WITH_YOUR_NGROK_AUTH_TOKEN)

