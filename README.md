# MammaTyper vs IHC Comparison — TFG Demo

Public demo of a web application developed as part of a **Bachelor's Thesis (TFG)** in Health Engineering at the **University of Burgos**.

The application allows automated **comparison between immunohistochemistry (IHC) results and molecular subtyping obtained with MammaTyper®** for breast cancer classification.

This repository contains a **demo version** of the system that can be executed locally or accessed online.

---

# Live Demo

You can access the public demo here:

https://tfg-mammatyper-demo.streamlit.app/

The demo includes **simulated and anonymized example files** to illustrate the functionality of the system without using real clinical data.

---

# Project Context

Breast cancer molecular subtyping is essential for guiding therapeutic decisions. In routine clinical practice, classification is commonly performed using **immunohistochemistry (IHC)** by evaluating biomarkers such as:

- ER (Estrogen Receptor)  
- PR (Progesterone Receptor)  
- HER2  
- Ki-67  

However, IHC can present limitations due to **inter-observer variability and subjective interpretation**, particularly for Ki-67.

The **MammaTyper® assay**, based on RT-qPCR, quantifies the expression of the genes:

- ESR1  
- PGR  
- ERBB2  
- MKI67  

This provides a **quantitative and reproducible molecular classification**.

The application developed in this project automates the integration and comparison of both methods.

---

# Features

The system allows:

- Import of IHC results from **Excel files (PatWin)**
- Import of **MammaTyper PDF reports**
- Automatic **biomarker extraction**
- Data integration into a structured dataset
- Identification of **concordances and discordances**
- Generation of structured reports
- Export of processed results

The application is implemented using **Python and Streamlit** to provide a simple interface suitable for clinical environments.

---

# Running the Demo Locally

Clone the repository:

```bash
git clone https://github.com/diegoalvrezz/TFG_MammaTyper_Demo.git
cd TFG_MammaTyper_Demo
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run the application:

```bash
streamlit run demo_app/demo_app.py
```

The app will open automatically in your browser.

---

# Demo Files

Example anonymized files are included in:

```
demo_app/demo_files
```

These files allow users to test the full workflow without requiring real hospital data.

---

# Repository Structure

```
TFG_MammaTyper_Demo
│
├── codigo/                 core processing modules
├── demo_app/               Streamlit demo application
│   ├── demo_app.py
│   └── demo_files/
│
├── requirements.txt
├── README.md
└── LICENSE
```

---

# Clinical Data Disclaimer

This repository **does not contain real clinical data**.

All files included in the demo are:

- simulated  
- anonymized  
- provided only for demonstration purposes  

The original application is designed to operate with **previously anonymized data in a hospital environment**.

---

# Author

Diego Vallina Álvarez  
Health Engineering Degree  
University of Burgos

Bachelor’s Thesis developed in collaboration with the **Hospital Universitario de Burgos (HUBU)**.

---

# License

This project is distributed under the **MIT License**.

See the `LICENSE` file for more information.
