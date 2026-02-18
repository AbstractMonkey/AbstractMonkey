# Hey, I'm Sean 👋

ML Engineer building systems that make healthcare better for real humans. Currently at a healthtech startup in Minneapolis where I design and ship production ML pipelines — patient clustering, lead scoring, sentiment analysis — serving millions of members across major insurance partners.

I come from a microbiology background, which means I think about complex systems a lot — whether that's cell signaling or figuring out why a patient clustering pipeline is producing continuous manifolds instead of discrete segments. The throughline is the same: observe carefully, model rigorously, iterate relentlessly.

**I love hard problems that live at the intersection of engineering craft and tangible impact.** The stuff I'm most proud of isn't always the most technically exotic — sometimes it's a well-designed RAG pipeline that gives leadership visibility they never had before, or a temporal windowing strategy that triples your usable training data overnight.

When I'm not working, I'm projecting 5.13 routes and sending V8 boulders, or building instruments that didn't exist yesterday.

---

### What I'm Working On

🥁 **[BeastBox](https://github.com/AbstractMonkey/BeastBox)** — Real-time beatbox-to-MIDI instrument  
A native C++/JUCE audio engine performs onset detection and ONNX inference at **sub-10ms latency**, connected to a cross-platform Flutter desktop UI via `dart:ffi` with a lock-free SPSC ring buffer. The real-time path — mic to UI — touches zero Python, zero network, zero heap allocations. Currently in alpha with a custom CNN classifier (98.4% accuracy, 0.035ms inference on a 3KB model). Future: VST/AU plugin, mobile, extended percussion classes.

📊 **CSAT Sentiment Analysis Pipeline** *(proprietary)*  
End-to-end pipeline that extracts healthcare call surveys from Redshift, runs hybrid NPS/sentiment analysis via AWS Bedrock (Claude), generates executive narratives with graceful fallbacks, and renders interactive Chart.js dashboards. Built with a custom survey compression layer achieving 60-70% token reduction while preserving sentiment signal. This one went from "side experiment" to "the CEO wants this in every board deck" in about three weeks.

🧠 **Patient Engagement Prediction** *(proprietary)*  
Production ML pipeline predicting patient engagement likelihood for targeted health interventions. The interesting bit: a bespoke temporal windowing approach with systematic lookback analysis (1–18 month windows), data quality tiering across 12 insurance groups, and outlier detection that caught members with 2M+ claims/month (yes, data issues). This windowing strategy dramatically expanded our viable training cohort and significantly improved AUC-PR. Supports both PyTorch neural nets and XGBoost, with full SageMaker orchestration and Bayesian HPO.

---

### Stack

```
Languages      Python · C++ · Dart · SQL
ML/AI          PyTorch · TensorFlow · XGBoost · scikit-learn · ONNX Runtime · AWS Bedrock
Data           dbt · Redshift · PostgreSQL · Pandas · Polars
Infrastructure AWS (SageMaker, Bedrock, S3, ECR) · Docker · Kubernetes · GitHub Actions
Audio/DSP      JUCE · librosa · FFTW
Frontend       Flutter · React
```

---

### Philosophy

I believe the best ML work happens when you care as much about the data pipeline as the model architecture. I'd rather spend a week getting the temporal windows right than chase marginal gains on hyperparameters with garbage training data.

I also believe production code should spark joy — for the people who use it *and* the people who maintain it. Good docs, clean abstractions, tests that actually test something, and CI that catches your mistakes before your teammates do.

---

### Let's Connect

📍 Minneapolis, MN  
💼 [LinkedIn](https://linkedin.com/in/seanhobin)  
📬 Open to conversations about healthcare ML, real-time audio, or your hardest clustering problem.
