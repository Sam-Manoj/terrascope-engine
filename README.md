# TerraScope: AI-Powered Botanical Diagnostics

**TerraScope** is an intelligent decision-support engine designed to bridge the gap between complex botanical health data and accessible, real-time remediation. By integrating computer vision and machine learning, TerraScope enables users to upload images of plant foliage to receive an instant diagnostic report, complete with severity metrics and organic treatment protocols.

## 🌟 The Vision

In an era of precision agriculture and home gardening, identifying early signs of nutrient deficiency or disease is often costly and time-consuming. TerraScope aims to democratize plant health management by providing an automated, "always-on" diagnostic expert accessible directly from a browser.

## 🛠️ Key Technical Capabilities

### 1. The Diagnostic Engine (TerraScope Engine)

The brain of the operation—a high-performance microservice built with **FastAPI**. It processes visual data using an ML-pipeline that includes:

* **Chromatic Analysis:** Utilizing `OpenCV` to perform real-time extraction of dominant color signatures from uploaded imagery.
* **Inference Pipeline:** A trained `Random Forest` model (powered by `scikit-learn`) classifies these color signatures against known botanical health markers.
* **Dynamic Knowledge Base:** A structured JSON database that returns context-aware remediation advice based on the model's prediction.

### 2. The Interactive Interface

The frontend is a bespoke **Next.js** application designed for efficiency and aesthetics:

* **Seamless Interaction:** Uses `Magic Bento` grids and `PixelTransition` animations to ensure a high-energy user experience.
* **Async Processing:** Implements a reactive data-fetching layer that handles the "cold-start" latency of cloud-hosted AI models gracefully.
* **Responsive Design:** Optimized for mobile and desktop, ensuring users can use the engine in the field or the greenhouse.

## 🏗️ Architecture

## 🚀 Deployment Status

TerraScope is built with a production-first mindset:

* **Containerization:** Fully Dockerized to ensure environment consistency.
* **Infrastructure:** Deployed using a split-stack architecture—hosting the frontend on Vercel for high-speed edge distribution and the diagnostic engine on Render for robust Python scaling.
* **Security:** Strict CORS middleware configuration ensures safe communication across the Vercel-Render bridge.

---


---
