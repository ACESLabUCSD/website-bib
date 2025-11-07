# 🧠 ACES Lab Website – Paper & Member Management Guide

This repository manages the **lab’s publication list** displayed on the official [ACES Lab Website](https://sites.google.com/ucsd.edu/aceslab/).  
The site automatically pulls data from this repo’s BibTeX file:  
👉 [**papers.bib**](https://github.com/ACESLabUCSD/website-bib/blob/main/papers.bib)

---

## 📂 Repository Overview

- **`papers.bib`** – Master BibTeX file containing all papers.
- **Google Drive Folder:**  
  [ACES Lab Website Drive Folder](https://github.com/ACESLabUCSD/website-bib/tree/main/Papers)
  - Contains subfolders by **year** for storing PDFs.
  - Each paper’s PDF must be uploaded here before linking.

---

## 🧾 How to Add or Update Papers

Follow these steps whenever adding a new paper or linking an existing one:

### 1️⃣ Upload the Paper PDF

Upload the paper to the correct **year folder** in the shared Github repository under /Papers/*YEAR*/*YOUR_PAPER*.

Make sure to commit this change, otherwise it will not display in the webpage.

### 2️⃣ Note the Path that was Saved to

Copy the filepath of:

/Papers/*YEAR*/*YOUR_PAPER*

### 3️⃣ Paste the Copied Path into the Tex below
url = {https://raw.githubusercontent.com/ACESLabUCSD/website-bib/refs/heads/main<PASTE COPIED PATH HERE>}



### 4️⃣ Insert the Tex from Step 3 into your Bibtex
In [`papers.bib`](https://github.com/ACESLabUCSD/website-bib/blob/main/papers.bib),  
find the corresponding paper entry and update its `url` field or paste the Tex into the Bibxtex entry:
```bibtex
@article{Aghazadeh2025ForTIFAI,
  title = {ForTIFAI: Fending Off Recursive Training Induced Failure for AI Model Collapse},
  author = {Soheil Zibakhsh Shabgahi and Pedram Aghazadeh and Azalia Mirhoseini and Farinaz Koushanfar},
  journal = {Under Review},
  year = {2025},
   url = {https://raw.githubusercontent.com/ACESLabUCSD/website-bib/refs/heads/main<INSERT_FULL_PATH_OF_PDF_FROM_PAPERS>}
}
That’s it! The website will automatically update to include the new paper and its downloadable PDF link.