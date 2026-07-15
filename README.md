## About Me

I am a Computer Science master's student at Saarland University, Germany, with a focus on machine learning, the security aspects of ML systems, and software testing.

Beyond academics, I am actively involved in voluntary work as a Mentee at Safe AI Germany, where I contribute to the field of Technical AI Safety.

In my free time, I enjoy playing badminton, table tennis, and solving logic puzzles.

## Projects

### Mini‑Cortex
Repository: https://github.com/Meenakshi04081999/mini-cortex

A rule‑based image inspection system designed to classify images as defect or non‑defect.
The project focuses on traditional computer vision logic rather than ML, making it suitable for industrial inspection pipelines where deterministic behavior is required.

Highlights:

Implemented rule‑based defect detection

Designed inspection logic for binary classification

Useful for manufacturing quality control workflows


### Membership Inference Attack - TML 2026

Repository: https://github.com/Meenakshi04081999/TrustworthyML_2026

This project performs a Membership Inference Attack on a ResNet‑18 model trained on a subset of a dataset.
The goal is to determine whether a given sample was part of the model’s training data (member) or not (non‑member) using only model outputs and confidence scores.

Key Concepts:

Privacy evaluation of ML models

Detecting information leakage through confidence scores, loss behavior, and internal representations

Assigning a membership likelihood score between 0 and 1

Final evaluation metric: TPR @ 5% FPR

Highlights:

Implemented a complete MIA pipeline

Analyzed model leakage behavior

Evaluated attack performance under strict low‑FPR constraints


### Adversarial Robustness

Repository: https://github.com/Meenakshi04081999/Adversarial-ML-Robustness-

This project builds a robust image classifier capable of correctly classifying both clean and adversarially perturbed images.
The dataset contains 50,000 labeled RGB images (3×32×32) across 9 classes.

Models used: ResNet‑18, ResNet‑34, ResNet‑50

Goal:  
Train a classifier that maintains high accuracy on both clean and adversarial inputs, despite unknown evaluation attacks.

Final Score: Score = 0.5 ⋅ clean accuracy + 0.5 ⋅ robust accuracy

Model must achieve >50% accuracy to be considered valid.

Techniques Used:

Data augmentation

Adversarial training

Optimization and fine‑tuning

Balancing clean accuracy vs robustness

Highlights:

Built a robust classifier resilient to multiple perturbation types

Improved adversarial robustness without sacrificing clean accuracy

Explored trade‑offs between model performance and security

### Watermark forgery attack

Repository: https://github.com/Meenakshi04081999/Watermark-Forgery-Attack-TML2026

This project attempts watermark forging: modifying clean images so they appear to contain a specific invisible watermark, without knowing how the watermark was originally generated.

You are given:

25 example images for each of eight unknown watermarking methods

200 clean target images to forge onto

Challenge:  
The forged images must satisfy two conditions simultaneously:

High bit accuracy  
→ The watermark detector must successfully read the forged watermark.

Low LPIPS distance  
→ The image must remain visually unchanged to the human eye.

Too strong → image looks damaged
Too weak → watermark does not register

Highlights:

Balanced watermark strength vs perceptual quality

Designed forgery strategies for eight watermarking schemes

Evaluated results using bit accuracy + LPIPS similarity

### PDF Integrated Enhanced Retrieval Question Answering system 

Project link: https://github.com/Meenakshi04081999/PIER_QA_2024/tree/master
Paper link: https://arxiv.org/abs/2506.18027

This project presents an advancement in Question answering systems using RAG framework to enhance information extraction from the PDF files. We introduce an end-to-end system that retrieves and processes images, diagrams, graphs, and tables embedded within PDF documents, extending beyond the capabilities of conventional text-centric RAG models. We also implement preprocessing steps including the removal of headers and footers, conversion of PDFs to markdown for easier manipulation, image captioning and table reformatting to enhance data readability and retrieval accuracy. Finally, we fine-tune language models to be RAG-aware, ensuring a better understanding of our data format and document domain.

### Outcome based distillation for jailbreaking safety guardrails

Project link: Work-in-progress

As model capabilities increase, safety guardrails are increasingly deployed to prevent malicious actors from extracting harmful information. While some mechanisms, such as model-level refusals, provide a rich feedback signal to an attacker, black-box input-level filters typically expose only a binary outcome. Recent work, “Boundary Point Jailbreaking of Black-Box LLMs,” demonstrated a fully automated attack pipeline against input filters, but requires up to 160K harmful queries before succeeding. In this project, we propose to frame guardrail jailbreaking as an outcome-based knowledge distillation problem, where the attacker iteratively approximates the guardrail by fine-tuning an off-the-shelf LLM-based classifier on observed outcomes. The goal of the project is to reduce the total harmful query budget required to successfully jailbreak a guardrail under this setting, and to study how this budget empirically depends on the level of information exposure provided by the guardrail.
