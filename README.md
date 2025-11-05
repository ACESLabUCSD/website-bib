# 🧠 ACES Lab Website – Paper & Member Management Guide

This repository manages the **lab’s publication list** displayed on the official [ACES Lab Website](https://sites.google.com/ucsd.edu/aceslab/).  
The site automatically pulls data from this repo’s BibTeX file:  
👉 [**papers.bib**](https://github.com/ACESLabUCSD/website-bib/blob/main/papers.bib)

---

## 📂 Repository Overview

- **`papers.bib`** – Master BibTeX file containing all papers.
- **Google Drive Folder:**  
  [ACES Lab Website Drive Folder](https://drive.google.com/drive/folders/1jd7NJ8zL6D5J1-CBzuiUMsUH4HlL13X2?usp=sharing)
  - Contains subfolders by **year** for storing PDFs.
  - Each paper’s PDF must be uploaded here before linking.

---

## 🧾 How to Add or Update Papers

Follow these steps whenever adding a new paper or linking an existing one:

### 1️⃣ Upload the Paper PDF
Upload the paper to the correct **year folder** in the shared Drive.

### 2️⃣ Get the Shareable Link
Right-click the uploaded PDF → “Get link.”  

### 3️⃣ Generate a Downloadable Link
Extract the **file ID** (the part between `/d/` and `/view`) and insert it here:
https://drive.google.com/uc?export=download&id=YOUR_FILE_ID
Example:
https://drive.google.com/uc?export=download&id=1vHmQnVetPFZAQb3xlXeFCRBIOalkNnko

> 💡 *Tip:* This can be automated with a short Python script to convert Google Drive links into downloadable links.  
> If anyone writes one, please share it in this repo!

### 4️⃣ Update the BibTeX Entry
In [`papers.bib`](https://github.com/ACESLabUCSD/website-bib/blob/main/papers.bib),  
find the corresponding paper entry and update its `url` field:
```bibtex
@article{Aghazadeh2025ForTIFAI,
  title = {ForTIFAI: Fending Off Recursive Training Induced Failure for AI Model Collapse},
  author = {Soheil Zibakhsh Shabgahi and Pedram Aghazadeh and Azalia Mirhoseini and Farinaz Koushanfar},
  journal = {Under Review},
  year = {2025},
  url = {https://drive.google.com/uc?export=download&id=1vHmQnVetPFZAQb3xlXeFCRBIOalkNnko}
}
That’s it! The website will automatically update to include the new paper and its downloadable PDF link.