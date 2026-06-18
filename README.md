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


