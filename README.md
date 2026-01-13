# VL-JEPA vs Traditional LLMs: Interactive Architecture Visualizer

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Status](https://img.shields.io/badge/status-Research%20Grade-green)

A high-fidelity, interactive system diagram comparing **Traditional Autoregressive LLMs** with **Meta's VL-JEPA** (Vision-Language Joint Embedding Predictive Architecture).

Designed for AI researchers, educators, and technical speakers to visually demonstrate the shift from **token generation** to **representation prediction**.

## 🚀 Live Visualization

> **[Click here to view the visualization locally](vl_jepa_vis.html)**  
*(If hosted on GitHub Pages, replace this with the live URL)*

## 🎯 Core Concept

This tool illustrates the fundamental philosophical difference in learning objectives:

| Feature | Traditional LLM | VL-JEPA |
| :--- | :--- | :--- |
| **Objective** | Predict next token $P(x_t | x_{<t})$ | Predict missing meaning $sim(pred(x), enc(y))$ |
| **Mechanism** | Autoregressive Loop | Joint Embedding Prediction |
| **Output** | Pixel/Token Sequence | Abstract Representation (z-vector) |
| **Compute** | O(n) Sequential | O(1) Parallel |

## ✨ Features

- **Research-Grade Aesthetics**: Styled after NeurIPS/CVPR system diagrams (Academic Grid, Inter/JetBrains Mono typography).
- **Dual-Column Simulation**:
  - **Left**: Live simulation of Transformer decoding, Softmax probabilities, and sequential loops.
  - **Right**: Live simulation of Image Masking, Dual Encoders (Context vs Target), and Latent Space Prediction.
- **Interactive Focus Mode**: Toggle between "Compare Both", "Focus LLM", and "Focus VL-JEPA" to guide audience attention during talks.
- **Architectural Accuracy**:
  - Visualizes the **Stop-Gradient / EMA** target encoder.
  - Shows explicit **L2/Cosine Loss** computation in embedding space.
  - Highlights the absence of decoding loops in JEPA.

## 🛠️ Tech Stack

- **HTML5**: Semantic structure.
- **Tailwind CSS**: Utility-first styling and complex animations.
- **Vanilla JavaScript**: Simulation logic and state management (Zero dependencies).
- **SVG**: Vector graphics for arrows and diagram elements.

## 📦 How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/vl-jepa-visualizer.git
   ```
2. Navigate to the folder:
   ```bash
   cd vl-jepa-visualizer
   ```
3. Open `vl_jepa_vis.html` in your browser (Chrome, Edge, Firefox).

## 🤝 Contributing

Contributions are welcome! If you want to add more architectures (e.g., Diffusion Models, I-JEPA) or improve the animations, feel free to open a PR.

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
