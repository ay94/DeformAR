# DeformAR: A Visual Analytics Framework for Interpretable NER Evaluation

**DeformAR** is a visual analytics and diagnostic framework designed to rethink how Named Entity Recognition (NER) systems are evaluated. It supports multilingual analysis, with case studies in Arabic and English, and enables researchers to explore model and data interactions through interactive, component-based visualizations.

---

## 🧩 Project Structure

DeformAR is organized into two modular libraries:

- **[deformar-extraction](https://github.com/ay94/deformar-extraction)**  
  A Python package for extracting diagnostic signals from both data and model subcomponents after NER fine-tuning. This includes token-level behavioural metrics (e.g., confidence, loss, entropy), as well as structural, lexical, and interaction metrics across the system’s components (e.g., tag inconsistency, tokenisation rate, OOV rates). Fully compatible with HuggingFace `transformers`.

- **[deformar-dashboard](https://github.com/ay94/deformar-dashboard)**  
  An interactive dashboard built with Plotly Dash for visualizing and interpreting NER model behavior through UMAP projections, scatter plots, token level analysis and attention maps.

---

## 💡 Key Features

- 📊 Cross-component evaluation using quantifiable metrics, interpretability techniques, and interactive visualizations
- 🌐 Multilingual support (Arabic and English tested)
- 🔍 Token-level insights (loss, entropy, confidence, label inconsistency)
- 🧠 Representation-space projections (UMAP, silhouette scores)
- ⚠️ Annotation error and calibration analysis
- 🧱 Modular design for flexible adaptation to other sequence labelling tasks

---

## 🚀 Getting Started

1. Clone the [extraction library](https://github.com/yourusername/deformar-extraction) and fine tune your model with your NER dataset to generate structured extraction outputs. These include subcomponent-level metrics and token-level behavioural metrics, which can be saved locally or directly to a Google Drive–compatible folder structure.
2. Use the [dashboard interface](https://github.com/yourusername/deformar-dashboard) to load these outputs and interactively visualize the system’s performance. The dashboard reads the saved extraction files and renders views across representation space, error types, and behavioural metrics.
3. Both libraries are configurable and designed for modular use. For installation, configuration, and usage details, please refer to the individual READMEs in each repository.
---

## 📝 Citation

If you use DeformAR in your work, please cite the following:

> Ahmed Mustafa Younes and Julie Weeds. *DeformAR: Rethinking NER Evaluation through Interpretability and Visual Analytics with Arabic and English as Case Studies*. Submitted to EMNLP 2025 (System Demonstrations Track).  
>
> A related PhD thesis was submitted to the University of Sussex in June 2025 and will be publicly available following final corrections.

---

## 📜 License

This project is licensed under the [Apache License 2.0](LICENSE).

---

## 🤝 Acknowledgments

DeformAR was developed as part of the PhD thesis "DeformAR: A Structured Evaluation and Diagnostic Framework for Sequence Labelling" at the University of Sussex. We thank the open-source community and the reviewers of the long paper version for their valuable feedback.

