# Personalized Face Detection & Recognition Using Ultralytics YOLO

A computer vision and machine learning project focused on detecting personalized human faces in images and real-time streams using Ultralytics YOLOv8n, deployed to an executive web application hosted on Vercel with dedicated Google Cloud Run inference.

---

## Project Overview

Face detection is a computer vision task that involves identifying the presence and bounding-box coordinates of human faces within an image or video frame. This project explores the training, evaluation, and deployment of a personalized face detection model using deep learning and the Ultralytics YOLO framework.

The primary objective is to build an efficient, mobile-accessible face detection system capable of identifying a target individual accurately across varying lighting conditions, backgrounds, facial expressions, and clothing styles.

### Objectives
* **Data Collection & Annotation:** Curate a custom dataset of 500+ images (individual and group photos) labeled in YOLO format.
* **Model Training:** Fine-tune a lightweight **YOLOv8n (Nano)** base model using the Ultralytics Platform.
* **Model Evaluation:** Measure precision, recall, mAP@50, and latency benchmarks.
* **Cloud Deployment:** Deploy a dedicated inference endpoint on Google Cloud Run.
* **Web & Mobile Application:** Build an inference studio web application deployed on Vercel for live testing and confidence tuning.

---

## Technologies and Tools

| Technology | Purpose |
| :--- | :--- |
| **Python** | Scripting, data pipeline, and evaluation |
| **Ultralytics YOLOv8n** | Computer vision architecture for face detection |
| **PyTorch** | Deep learning framework underlying YOLO |
| **Google Cloud Run** | Dedicated serverless container hosting the inference engine |
| **HTML5 Canvas / JS** | Real-time bounding box rendering and live parameter controls |
| **Tailwind CSS** | Dashboard UI design inspired by modern analytics interfaces |
| **Vercel** | Web application hosting and CDN distribution |
| **Git / GitHub** | Version control and academic project documentation |

---

## Live Inference Endpoint

The model is hosted on a dedicated Google Cloud Run instance:
* **Inference URL:** `https://predict-6b08f46b1522388bcc62ddd7-dproatj77a-nw.a.run.app/predict`
* **API Documentation:** `https://predict-6b08f46b1522388bcc62ddd7-dproatj77a-nw.a.run.app/docs`

---

## Running the Web App Locally

1. Clone the repository:
   ```bash
   git clone https://github.com/TheProfSam/Face-detection-.git
   cd Face-detection-
   ```

2. Start a local HTTP server:
   ```bash
   python -m http.server 3000
   ```

3. Open **`http://localhost:3000`** in your browser.

---

## Deploying to Vercel

The project includes `vercel.json` for zero-configuration deployment:

### Option 1: Via Vercel CLI
```bash
npx vercel
```

### Option 2: Via Vercel Dashboard
1. Go to [vercel.com](https://vercel.com).
2. Click **Add New...** → **Project**.
3. Import the `TheProfSam/Face-detection-` repository.
4. Click **Deploy**.
