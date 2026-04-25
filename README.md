Image Forensic Suite
Explainable AI for Document Forgery Detection

An advanced AI-powered Image Forensic Suite that goes beyond traditional OCR by performing a multi-layered forensic analysis to detect digital manipulation in documents.

Overview

This project combines image processing, OCR, and statistical analysis to identify hidden signs of tampering in documents such as receipts, certificates, and IDs.

Unlike basic OCR tools (e.g., Tesseract OCR), this system performs a deep forensic audit to uncover inconsistencies in both image structure and extracted text.

🧠 Key Features
🔍 1. Intelligent Image Pre-processing
Dynamic Upscaling (1400px–2400px) for better OCR accuracy
Contrast Enhancement (1.35×) for improved readability
Grayscale Conversion to remove color noise
🔬 2. OpenCV-style Image Forensics

Inspired by techniques from OpenCV

Laplacian Variance → Detects blur (possible intentional obfuscation)
Sobel Edge Analysis → Identifies artificial text insertion
Blockiness Detection → Finds inconsistent JPEG compression artifacts
Channel Spread Analysis → Flags unnatural color manipulation
📊 3. Explainable AI Insights

Transforms raw metrics into human-readable explanations:

Exposure → Overexposed / Underexposed
Sharpness → Sharp / Blurry
Color Profile → Flat / Harsh
🔍 4. OCR Statistical Auditing

Deep analysis of extracted text:

P10 (10th Percentile) Confidence Check → Detects weak regions
Outlier Detection → Flags abnormal words
Noise Filtering → Removes low-confidence short tokens
Keyword Blacklist Scan → Detects hidden words like Edited, Photoshop, Forgery
🌍 5. Multi-format & Multilingual Support
📄 PDF support via canvas rasterization
🌐 Multi-language OCR (e.g., English + Tamil)
⚡ Performance optimization for language packs
💾 Persistent user settings via local storage
⚖️ 6. Risk Scoring Engine

A dynamic scoring system that:

Combines image forensics + OCR signals
Adjusts weights based on text density
Outputs a final Forgery Risk Score (0–100)
🔐 7. Security & Reliability
XSS Protection for safe text rendering
Average Hashing (AHash) for duplicate detection
Secure client-side processing
🛠️ Tech Stack
Frontend: HTML, CSS, JavaScript
OCR Engine: Tesseract.js
Image Processing: Canvas API + custom OpenCV-style algorithms
PDF Handling: Canvas-based rasterization
Storage: Browser LocalStorage
📈 Use Cases
🏦 Banking & Financial Document Verification
🧾 Receipt & Invoice Fraud Detection
🏛️ Government Document Validation
⚖️ Legal Evidence Screening
