## Hi, I'm Martín 👋

Fourth-year **AI Engineering** student at Universidad de San Andrés, Buenos Aires, doing AI and process automation at Aleph. Open to **AI/ML engineering internships and junior roles**.

I build machine learning systems end to end — dataset, model, evaluation, demo — across **computer vision, NLP and LLMs, speech and audio, and robotics**. The part I care about most is the evaluation: paired bootstrap with 95% CIs, speaker-independent splits, negative results reported as findings. Two of the projects below are ones where the method I was testing didn't win.

---

### Selected projects

**[Visual Speech Recognition for Rioplatense Spanish](https://github.com/mateobramer/labios-argentos)** · *team of 5 · repo on a teammate's account*
No public lipreading corpus existed for this Spanish variant, so we built one: **~12,100 lip clips / ~19 h** from YouTube, 96.34% quality retention, frozen splits and a **speaker-independent** test with two held-out speakers. Fine-tuned 50M–288M-parameter VSR models (full FT vs LoRA), then ran a standardised 13-cell grid on LLM rescoring with paired bootstrap (5,000 resamples) and 95% CIs.
**The headline is the negative result:** LLM **1-best correction significantly hurts in 9 of the 13 settings** — it "corrects" transcriptions that were already right. **5-best reranking helps only on clean material** (**−2.81 WER, 95% CI [0.86, 4.77]**, selftest-150 pool), with **no effect** on YouTube material. Test references are machine-generated, so the WER is an upper bound on true error. Working live demo included.

**[VisionTrafficGuard](https://github.com/martinbianchi0/VisionTrafficGuard)** · *team of 3*
Video-only traffic enforcement: YOLOv11 + ByteTrack, per-lane homography speed estimation, plate OCR with temporal voting. **0.77 km/h speed MAE** with radar-calibrated homographies (N=64) versus **3.60 km/h** with self-calibration needing only a 4.4 m reference (N=387) — the accuracy-vs-deployability trade-off, quantified.

**[Do generative models help imbalanced audio classification?](https://github.com/martinbianchi0/whale_challenge)** · *team of 2*
A controlled negative result. Trained a VAE, an AAE and a GAN to synthesise whale-call spectrograms; **none improved the F1 of a classifier trained on real data alone** (baseline F1 0.8471, best synthetic 0.8384). Reported as the finding, not buried.

**[Autonomous maze-running robot](https://github.com/martinbianchi0/robot_maze_runner)** · *team of 4*
Five ROS 2 packages: FastSLAM, Monte Carlo localization, A\* planning and a mission state machine. Developed in simulation and **validated on real TurtleBot4 hardware** — including finding the LIDAR was physically mounted 90° off. Cone detector: **0 false positives over 1,798 manually reviewed frames**.

**[End-to-end data platform](https://github.com/damiandistefano/tp-arquitectura-oilgas)** · *team of 3 · repo on a teammate's account*
Medallion warehouse with Dagster and dbt, MLflow registry with a promotion gate, drift detection, FastAPI + Docker, CI/CD to AWS. Three phases, documented with architecture decision records.

---

### Also worth a look

**[Probabilistic robotics from scratch](https://github.com/martinbianchi0/probabilistic-robotics-from-scratch)** — Bayes filter, MCL, both EKF Jacobians, Rao-Blackwellized FastSLAM, six planners compared, with **per-stage provenance separating course scaffolding from my own code** · **[Classical computer vision](https://github.com/martinbianchi0/Vision-Learning)** — **homography written from scratch** (DLT via SVD + hand-rolled RANSAC), not `cv2.findHomography` · **[ML from scratch](https://github.com/martinbianchi0/Machine-Learning)** — an MLP with backpropagation and ADAM; **no scikit-learn, the assignment forbade ML libraries** · **[mlflow casero](https://github.com/martinbianchi0/mlflow-casero)** — a PostgreSQL schema where reproducibility is enforced by database constraints, not documentation

---

### Stack

**Core** — Python · PyTorch (+ Lightning) · NumPy / SciPy · pandas · scikit-learn · OpenCV · SQL / PostgreSQL · Docker & Compose · FastAPI · ROS 2 · Git & PR review · pytest · GitHub Actions

**Also worked with** — C · x86-64 & ARM assembly · Java · Haskell · LoRA / PEFT · ESPnet · Whisper · librosa · Ultralytics YOLO · ByteTrack · Open3D · MediaPipe · OCR (FastPlate, EasyOCR, Tesseract) · MLflow · Dagster · dbt · Spark · Neo4j · AWS EC2 · GCP · Prometheus / Grafana · Metabase · n8n · TurtleBot4

📍 Buenos Aires, Argentina · 💼 [LinkedIn](https://www.linkedin.com/in/martin-bianchi0/) · ✉️ bianchis.martin@gmail.com
