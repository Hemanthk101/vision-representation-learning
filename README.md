# Vision Representation Learning for Classification and Image Generation

## 📌 Overview
This project focuses on learning **transferable visual representations** using deep learning–based computer vision models and reusing those representations for downstream generative tasks. A Convolutional Neural Network (CNN) is trained to perform image classification while simultaneously learning meaningful feature embeddings. These learned features are then explored in the context of generative modeling using **Generative Adversarial Networks (GANs)** and **Diffusion Models**.

The project emphasizes **research correctness, reproducibility, and modular design**, rather than application-level demos.

---

## 🧠 Objectives
- Learn robust visual feature representations from images
- Train a CNN for image classification and feature extraction
- Reuse learned representations for generative modeling
- Evaluate models using both quantitative and qualitative methods
- Maintain a clean, extensible, research-oriented project structure

---


---

## 🗂 Dataset
A custom-organized image dataset is used for experimentation.  
The pipeline includes:
- Image resizing and normalization
- Structured train/validation/test splits
- Dataset abstraction via PyTorch `DataLoader`

The structure supports easy replacement with larger or domain-specific datasets.

---

## 🏗 Methodology

### 1. Feature Learning (CNN)
- A CNN is trained for image classification
- Intermediate layers are used to extract feature embeddings
- Learned features capture semantic and structural image information

### 2. Representation Reuse
- CNN embeddings are reused as inputs or conditioning signals
- Enables experimentation beyond classification

### 3. Generative Modeling
- **GANs**: Use learned representations to guide image generation
- **Diffusion Models**: Explore conditional and guided generation using embeddings

---

## 📊 Evaluation

### Quantitative Evaluation
- Accuracy
- Precision
- Recall
- Training vs. validation loss analysis

### Qualitative Evaluation
- Visual inspection of generated images
- Comparison of real vs. generated samples

---

## 🧪 Experiments
All experiments are documented through Jupyter notebooks to support:
- Interactive experimentation
- Visualization
- Reproducibility

Each notebook focuses on a single stage of the pipeline.

---

## ⚙️ Tech Stack
- Python
- PyTorch & Torchvision
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

---

## ▶️ How to Run

### Install dependencies
```bash
pip install -r requirements.txt

