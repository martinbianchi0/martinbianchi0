## Hi, I'm Martín 👋

Fourth-year **AI Engineering** student at Universidad de San Andrés, Buenos Aires. AI and process automation at Aleph.

End-to-end ML systems — dataset, model, evaluation, demo — across **computer vision, NLP and LLMs, speech and audio, and robotics**.

---

### Projects

**[Visual Speech Recognition for Rioplatense Spanish](https://github.com/mateobramer/labios-argentos)** · *team of 5 · teammate's repo*
No public lipreading corpus existed for this variant, so we built one: **~12,100 clips / ~19 h**, frozen splits, speaker-independent test. Fine-tuned 50M–288M-parameter VSR models (full FT vs LoRA), then a 13-cell LLM-rescoring grid with paired bootstrap and 95% CIs.
**1-best LLM correction hurts in 9 of the 13 settings** — it "fixes" transcriptions that were already right. 5-best reranking helps **only on clean material** (**−2.81 WER, 95% CI [0.86, 4.77]**, n=150), no effect on YouTube. References are machine-generated, so the WER is an upper bound. Live demo.

**[VisionTrafficGuard](https://github.com/martinbianchi0/VisionTrafficGuard)** · *team of 3*
Video-only traffic enforcement: YOLOv11 + ByteTrack, per-lane homography speed estimation, plate OCR. **0.77 km/h MAE** radar-calibrated (N=64) vs **3.60 km/h** self-calibrated off a 4.4 m reference (N=387) — accuracy vs deployability, quantified.

**[Generative augmentation for imbalanced audio](https://github.com/martinbianchi0/whale_challenge)** · *team of 2*
VAE, AAE and GAN synthesising whale-call spectrograms: **none beat real data alone** (baseline F1 0.8471, best synthetic 0.8384). Negative result, reported as the finding.

**[Autonomous maze-running robot](https://github.com/martinbianchi0/robot_maze_runner)** · *team of 4*
Five ROS 2 packages: FastSLAM, MCL, A\* planning, mission state machine. **Validated on real TurtleBot4** — including finding the LIDAR mounted 90° off. Cone detector: **0 false positives over 1,798 reviewed frames**.

**[End-to-end data platform](https://github.com/damiandistefano/tp-arquitectura-oilgas)** · *team of 3 · teammate's repo*
Medallion warehouse with Dagster and dbt, MLflow registry with a promotion gate, drift detection, FastAPI, CI/CD to AWS.

---

### Coursework

- **[Probabilistic robotics from scratch](https://github.com/martinbianchi0/probabilistic-robotics-from-scratch)** — Bayes filter, MCL, both EKF Jacobians, FastSLAM, six planners compared. **Per-stage provenance separating the course's scaffolding from my own code.**
- **[Classical computer vision](https://github.com/martinbianchi0/Vision-Learning)** — three projects: segmentation and counting (Otsu, morphology, distance-transform splitting) · panoramas with **the homography written from scratch** (DLT via SVD + own RANSAC, not `cv2.findHomography`; OpenCV only detects and warps) · stereo 3D. Segmentation individual, panoramas in a pair.
- **[ML from scratch](https://github.com/martinbianchi0/Machine-Learning)** — four individual assignments, **no scikit-learn because the assignment forbade it**: regression (linear, Ridge, Lasso), classification (logistic, LDA, random forest), **an MLP with backpropagation and ADAM validated against PyTorch**, unsupervised (K-means, GMM, DBSCAN, PCA) and a VAE.
- **[mlflow casero](https://github.com/martinbianchi0/mlflow-casero)** — a PostgreSQL schema enforcing ML reproducibility through constraints, not documentation.

---

### Stack

**Core** — Python · PyTorch · NumPy / SciPy · pandas · scikit-learn · OpenCV · SQL / PostgreSQL · Docker · FastAPI · ROS 2 · Git · pytest · GitHub Actions

**Also** — C · x86-64 & ARM assembly · Java · Haskell · LoRA / PEFT · ESPnet · Whisper · librosa · YOLO · ByteTrack · Open3D · MediaPipe · OCR · MLflow · Dagster · dbt · Spark · Neo4j · AWS · GCP · Prometheus / Grafana · Metabase · n8n

📍 Buenos Aires, Argentina · [LinkedIn](https://www.linkedin.com/in/martin-bianchi0/) · bianchis.martin@gmail.com
