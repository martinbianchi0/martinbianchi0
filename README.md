## Hi, I'm Martín 👋

Fourth-year **AI Engineering** student at Universidad de San Andrés, Buenos Aires.

Most of what I build is computer vision and multimodal systems — detection and tracking, stereo geometry, speech and audio — and usually end to end: the data pipeline, the model and the evaluation. Currently working on AI and process automation at Aleph.

---

### Selected projects

**[Visual Speech Recognition for Rioplatense Spanish](https://github.com/mateobramer/labios-argentos)** · *team of 5 — hosted on a teammate's account*
Lipreading for a low-resource Spanish variant. Built a **19-hour dataset (~12,100 lip clips)** mined from YouTube, fine-tuned 50M–288M-parameter VSR models (full FT vs LoRA), and wrote an academic paper on **when LLM rescoring helps and when it hurts**: 5-best rescoring cut WER by **2.81 points (95% CI [0.86, 4.77])**, while 1-best correction *degraded* accuracy in 9 of 13 settings. Includes a working live demo.

**[VisionTrafficGuard](https://github.com/martinbianchi0/VisionTrafficGuard)** · *team of 3*
Video-only traffic enforcement: YOLOv11 + ByteTrack, per-lane homography speed estimation, plate OCR with temporal voting, infraction classification. **0.77 km/h speed MAE** with radar-calibrated homographies (N=64) versus **3.60 km/h** with self-calibration needing only a 4.4 m reference (N=387) — the accuracy-vs-deployability trade-off, quantified.

**[End-to-end data platform](https://github.com/damiandistefano/tp-arquitectura-oilgas)** · *team of 3 — hosted on a teammate's account*
FastAPI + Docker + CI/CD to AWS, a Medallion warehouse with Dagster and dbt, MLflow model registry with a promotion gate, drift detection and observability. Three phases, documented with architecture decision records.

**[Autonomous maze-running robot](https://github.com/martinbianchi0/robot_maze_runner)** · *team of 4*
Five ROS 2 packages: FastSLAM, Monte Carlo localization, A\* planning and a mission state machine. Developed in simulation and **validated on real TurtleBot4 hardware** — including finding that the LIDAR was physically mounted 90° off. Cone detector: **0 false positives over 1,798 manually reviewed frames**.

**[Do generative models help imbalanced audio classification?](https://github.com/martinbianchi0/whale_challenge)** · *team of 2*
A controlled negative result. Trained a VAE, an AAE and a GAN to synthesise whale-call spectrograms; **none of the three improved the F1 of a classifier trained on real data alone** (baseline F1 0.8471, best synthetic 0.8384). Reported as the finding, not buried.

---

### Coursework worth a look

- **[Classical computer vision](https://github.com/martinbianchi0/Vision-Learning)** — panoramas, segmentation and stereo 3D reconstruction, with **homography estimation written from scratch** (DLT via SVD + a hand-rolled RANSAC), not `cv2.findHomography`.
- **[ML from scratch](https://github.com/martinbianchi0/Machine-Learning)** — regression, classification, an MLP with backpropagation and ADAM, and unsupervised methods. **No scikit-learn: the assignment forbade ML libraries.**
- **[mlflow casero](https://github.com/martinbianchi0/mlflow-casero)** — a PostgreSQL schema for ML experiment traceability, where reproducibility is enforced by constraints rather than documentation.

---

### Stack

**Languages** · Python · C · SQL · x86-64 & ARM assembly · Java · Haskell

**ML & deep learning** · PyTorch (+ Lightning) · scikit-learn · NumPy / SciPy · pandas · LoRA / PEFT · ESPnet · Whisper · librosa · Matplotlib / seaborn

**Computer vision** · OpenCV · Ultralytics YOLO · ByteTrack · Open3D · MediaPipe · OCR (FastPlate, EasyOCR, Tesseract)

**Data & infrastructure** · PostgreSQL · Docker & Compose · FastAPI · Dagster · dbt · MLflow · Spark · Neo4j · AWS EC2 · GCP · Prometheus / Grafana · Metabase · n8n

**Robotics** · ROS 2 · TurtleBot4 · SLAM, localization and path planning

**Practices** · Git and PR review · pytest · GitHub Actions CI/CD · TDD and design patterns · technical writing

---

📍 Buenos Aires, Argentina · 💼 [LinkedIn](https://www.linkedin.com/in/martin-bianchi0/) · ✉️ bianchis.martin@gmail.com
